---
title: Développer des groupes de distribution à l’aide d’EWS Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Découvrez comment développer un groupe de distribution à l’aide de l’API gérée EWS ou EWS dans Exchange.
ms.openlocfilehash: 6aeebbd14604295bce46049f0e383663414c01a0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513184"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Développer des groupes de distribution à l’aide d’EWS Exchange 2013

Découvrez comment développer un groupe de distribution à l’aide de l’API gérée EWS ou EWS dans Exchange.
  
Vous pouvez utiliser la méthode d’API gérée EWS [ExchangeService.ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou l’opération [EWS ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour développer un groupe de distribution afin d’identifier tous les destinataires. 
  
Étant donné que [la méthode ExpandGroup](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) est surchargée, vous pouvez l’appeler de plusieurs manières : 
  
- [ExpandGroup(String)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx) : développe un groupe identifié par une adresse SMTP. 
    
- [ExpandGroup(EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) : développe un groupe identifié par une adresse de messagerie. 
    
- [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) : développe un groupe identifié par un ID de groupe. 
    
- [ExpanGroup(String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx) : développe un groupe identifié par une adresse SMTP et le type de routage de cette adresse. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Développer un groupe de distribution universel ou un groupe de sécurité à l’aide de l’API gérée EWS
<a name="bk_ExpandDGEWSMA"> </a>

L’exemple suivant montre comment développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’une adresse de messagerie, qui est l’approche la plus simple. Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Ce n’est pas beaucoup de code, mais il est également assez simple et peut ne pas vous donner ce que vous recherchez. Nous allons donc aller plus loin. Les groupes de distribution peuvent également contenir d’autres groupes de distribution. Le simple fait de l’étendre produit l’adresse e-mail des groupes de distribution contenus, mais pas de les développer. En ajoutant quelques lignes de code, vous pouvez développer de manière récursive les groupes pour obtenir la sortie de chaque contact.
  
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

Vous pouvez maintenant appeler cette nouvelle fonction dans votre code et développer tous les groupes de distribution publics contenus dans le premier.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Développer un groupe de contacts à l’aide de l’API gérée EWS
<a name="bk_ExpandDGEWSMA"> </a>

Étant donné que les groupes de contacts n’ont pas d’adresse de messagerie associée, vous devez développer le groupe en fonction de l’ItemId à l’aide de la méthode [ExpandGroup(ItemId).](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) Vous pouvez créer une fonction, comme illustré dans l’exemple précédent, et modifier le deuxième type de paramètre d’une chaîne en [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
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

Vous pouvez maintenant appeler cette fonction à l’aide de l’Exchange service et de **l’ItemId** du groupe de contacts. Notez que **l’élément ItemId** de l’exemple est raccourci pour des raisons de lisibilité. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’EWS
<a name="bk_ExpandDGEWSMA"> </a>

L’exemple suivant montre le message de demande XML qui est envoyé du client au serveur lorsque vous utilisez [l’opération ExpandDL.](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous utilisez l’API gérée EWS pour développer [un groupe de distribution universel.](#bk_ExpandDGEWSMA) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre le message de réponse XML envoyé du serveur au client. Notez que les boîtes aux lettres et les groupes de distribution universels sont renvoyés.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Contrairement à l’UTILISATION de l’API gérée EWS, lorsque vous utilisez EWS pour développer un groupe de distribution universel, vous ne pouvez pas développer de manière récursive les groupes de distribution renvoyés. Vous devrez envoyer une demande supplémentaire pour développer chacun des groupes de distribution inclus dans la réponse.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Développer un groupe de contacts à l’aide d’EWS
<a name="bk_ExpandDGEWSMA"> </a>

La demande XML de développement d’un groupe de contacts est similaire à une demande de développement d’un groupe de distribution. Au lieu d’une adresse de messagerie, vous utilisez [l’ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du groupe de contacts. Dans **cet exemple, l’élément ItemId** est raccourci pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

La structure de la réponse XML à une demande de développement d’un groupe de contacts est identique à la réponse à une demande de développement d’un groupe de distribution universel.
  
## <a name="see-also"></a>Voir aussi


- [Les groupes de distribution et EWS dans Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Créer des groupes de contacts à l’aide d’EWS dans Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

