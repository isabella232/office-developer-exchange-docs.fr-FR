---
title: Développez les groupes de distribution à l’aide EWS dans Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Découvrez comment développer un groupe de distribution à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754826"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Développez les groupes de distribution à l’aide EWS dans Exchange 2013

Découvrez comment développer un groupe de distribution à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez utiliser la méthode d’API managées [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour développer un groupe de distribution pour identifier tous les destinataires. 
  
[Expandgroup,](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) de la méthode est surchargé, vous pouvez l’appeler de plusieurs façons : 
  
- [ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse SMTP. 
    
- [ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse de messagerie. 
    
- [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - développe un groupe identifié par un ID de groupe. 
    
- [ExpanGroup (String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse SMTP et le type de routage de l’adresse. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Développez un groupe de distribution universel ou un groupe de sécurité à l’aide des API managées
<a name="bk_ExpandDGEWSMA"> </a>

L’exemple suivant montre comment développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’une adresse de messagerie, qui est l’approche la plus simple. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Ce n’est pas beaucoup de code, mais il est également élémentaire et peuvent ne pas vous donne à ce que vous recherchez. Examinons franchir une étape supplémentaire. Groupes de distribution peuvent également contenir d’autres groupes de distribution. Étendre simplement sera de sortie de l’adresse de messagerie des groupes de distribution de contenu mais pas les développer. En ajoutant quelques lignes de code, vous pouvez de manière récursive développer les groupes pour chaque contact de sortie.
  
```cs
private static void ExpandDistributionLists(ExchangeService service, string Mailbox)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(Mailbox);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         // Check to see if the mailbox is a public group
         if (address.MailboxType == MailboxType.PublicGroup)
      {
         // Call the function again to expand the contained
         // distribution group.
         ExpandDistributionLists(service, address.Address);
      }
      else
      {
         // Output the address of the mailbox.
         Console.WriteLine("Email Address: {0}", address);
      }
   }
}

```

Et maintenant, vous pouvez appeler cette nouvelle fonction le votre code et développer tous les groupes de distribution publiques contenues dans le premier.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Développez un groupe de contacts à l’aide des API managées
<a name="bk_ExpandDGEWSMA"> </a>

Étant donné que les groupes de contacts n’ont pas d’une adresse de messagerie associée, vous devez développer le groupe en fonction de l’ID d’élément à l’aide de la méthode [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) . Vous pouvez créer une fonction, comme indiqué dans l’exemple précédent et modifier le type de paramètre deuxième à partir d’une chaîne à un [ID d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
```cs
private static void ExpandContactGroup(ExchangeService service, ItemId groupID)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(groupID);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         if (address.MailboxType == MailboxType.PublicGroup)
         {
            ExpandDistributionLists(service, address.Address);
         }
         else
         {
            Console.WriteLine("Email Address: {0}", address);
         }
      }
}
```

Maintenant, vous pouvez appeler cette fonction à l’aide de l’objet de service Exchange et l' **ItemId** de groupe de contacts. Notez que l' **ID d’élément** dans l’exemple est réduit pour une meilleure lisibilité. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Développez un groupe de distribution universel ou un groupe de sécurité à l’aide de EWS
<a name="bk_ExpandDGEWSMA"> </a>

L’exemple suivant affiche le message de demande XML qui est envoyé à partir du client sur le serveur lorsque vous utilisez l’opération [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) . C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [développer un groupe de distribution universel](#bk_ExpandDGEWSMA). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant affiche le message de réponse XML qui est envoyé à partir du serveur au client. Notez que les boîtes aux lettres et des groupes de distribution universels sont retournés.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Support</Name>
          <EmailAddress>support@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
      </DLExpansion>
    </ExpandDLResponseMessage>
  </ResponseMessages>
</ExpandDLResponse>
</s:Body>
</s:Envelope>
```

Contrairement à lorsque vous utilisez l’API managée EWS, lorsque vous utilisez EWS pour développer un groupe de distribution universel, vous ne pouvez pas de manière récursive développer les groupes de distribution sont renvoyés. Vous devez envoyer une demande supplémentaire afin de développer chacun des groupes de distribution inclus dans la réponse.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Développez un groupe de contacts à l’aide de EWS
<a name="bk_ExpandDGEWSMA"> </a>

La demande XML pour développer un groupe de contacts est similaire à une demande pour développer un groupe de distribution. Au lieu d’une adresse de messagerie, vous utilisez l' [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de groupe de contacts. L' **ID d’élément** dans cet exemple est réduite pour une meilleure lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

La structure de la réponse XML à une demande pour développer un groupe de contacts est la même que la réponse à une demande pour développer un groupe de distribution universel.
  
## <a name="see-also"></a>Voir aussi


- [Les groupes de distribution et EWS dans Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Créer des groupes de contacts à l’aide de EWS dans Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

