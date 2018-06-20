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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754826"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a><span data-ttu-id="07180-103">Développez les groupes de distribution à l’aide EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="07180-103">Expand distribution groups by using EWS in Exchange 2013</span></span>

<span data-ttu-id="07180-104">Découvrez comment développer un groupe de distribution à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="07180-104">Learn how to expand a distribution group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="07180-105">Vous pouvez utiliser la méthode d’API managées [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour développer un groupe de distribution pour identifier tous les destinataires.</span><span class="sxs-lookup"><span data-stu-id="07180-105">You can use the [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS operation to expand a distribution group to identify all recipients.</span></span> 
  
<span data-ttu-id="07180-106">[Expandgroup,](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) de la méthode est surchargé, vous pouvez l’appeler de plusieurs façons :</span><span class="sxs-lookup"><span data-stu-id="07180-106">Because the [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) method is overloaded, you can call it in several ways:</span></span> 
  
- <span data-ttu-id="07180-107">[ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="07180-107">[ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address.</span></span> 
    
- <span data-ttu-id="07180-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="07180-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - Expands a group identified by an email address.</span></span> 
    
- <span data-ttu-id="07180-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - développe un groupe identifié par un ID de groupe.</span><span class="sxs-lookup"><span data-stu-id="07180-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - Expands a group identified by a group ID.</span></span> 
    
- <span data-ttu-id="07180-110">[ExpanGroup (String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - développe un groupe identifié par une adresse SMTP et le type de routage de l’adresse.</span><span class="sxs-lookup"><span data-stu-id="07180-110">[ExpanGroup(String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address and the routing type of that address.</span></span> 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a><span data-ttu-id="07180-111">Développez un groupe de distribution universel ou un groupe de sécurité à l’aide des API managées</span><span class="sxs-lookup"><span data-stu-id="07180-111">Expand a universal distribution group or security group by using EWS Managed API</span></span>
<span data-ttu-id="07180-112"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="07180-112"></span></span>

<span data-ttu-id="07180-113">L’exemple suivant montre comment développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’une adresse de messagerie, qui est l’approche la plus simple.</span><span class="sxs-lookup"><span data-stu-id="07180-113">The following example shows how to expand a universal distribution group or security group by using an email address, which is the simplest approach.</span></span> <span data-ttu-id="07180-114">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07180-114">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

<span data-ttu-id="07180-115">Ce n’est pas beaucoup de code, mais il est également élémentaire et peuvent ne pas vous donne à ce que vous recherchez.</span><span class="sxs-lookup"><span data-stu-id="07180-115">That's not a lot of code, but it's also pretty basic and might not give you what you are looking for.</span></span> <span data-ttu-id="07180-116">Examinons franchir une étape supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="07180-116">So let's take it a step further.</span></span> <span data-ttu-id="07180-117">Groupes de distribution peuvent également contenir d’autres groupes de distribution.</span><span class="sxs-lookup"><span data-stu-id="07180-117">Distribution groups can also contain other distribution groups.</span></span> <span data-ttu-id="07180-118">Étendre simplement sera de sortie de l’adresse de messagerie des groupes de distribution de contenu mais pas les développer.</span><span class="sxs-lookup"><span data-stu-id="07180-118">Simply expanding it will output the email address of the contained distribution groups but not expand them.</span></span> <span data-ttu-id="07180-119">En ajoutant quelques lignes de code, vous pouvez de manière récursive développer les groupes pour chaque contact de sortie.</span><span class="sxs-lookup"><span data-stu-id="07180-119">By adding a few more lines of code, you can recursively expand the groups to output every contact.</span></span>
  
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

<span data-ttu-id="07180-120">Et maintenant, vous pouvez appeler cette nouvelle fonction le votre code et développer tous les groupes de distribution publiques contenues dans le premier.</span><span class="sxs-lookup"><span data-stu-id="07180-120">And now you can call this new function in the your code and expand all the public distribution groups contained within the first one.</span></span>
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a><span data-ttu-id="07180-121">Développez un groupe de contacts à l’aide des API managées</span><span class="sxs-lookup"><span data-stu-id="07180-121">Expand a contact group by using EWS Managed API</span></span>
<span data-ttu-id="07180-122"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="07180-122"></span></span>

<span data-ttu-id="07180-123">Étant donné que les groupes de contacts n’ont pas d’une adresse de messagerie associée, vous devez développer le groupe en fonction de l’ID d’élément à l’aide de la méthode [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="07180-123">Because contact groups do not have an associated email address, you need to expand the group based on the ItemId by using the [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="07180-124">Vous pouvez créer une fonction, comme indiqué dans l’exemple précédent et modifier le type de paramètre deuxième à partir d’une chaîne à un [ID d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="07180-124">You can create a function, as shown in the previous example, and change the second parameter type from a string to an [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span></span>
  
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

<span data-ttu-id="07180-125">Maintenant, vous pouvez appeler cette fonction à l’aide de l’objet de service Exchange et l' **ItemId** de groupe de contacts.</span><span class="sxs-lookup"><span data-stu-id="07180-125">Now you can call this function by using the Exchange service object and the **ItemId** of the contact group.</span></span> <span data-ttu-id="07180-126">Notez que l' **ID d’élément** dans l’exemple est réduit pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="07180-126">Note that the **ItemId** in the example is shortened for readability.</span></span> 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a><span data-ttu-id="07180-127">Développez un groupe de distribution universel ou un groupe de sécurité à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07180-127">Expand a universal distribution group or security group by using EWS</span></span>
<span data-ttu-id="07180-128"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="07180-128"></span></span>

<span data-ttu-id="07180-129">L’exemple suivant affiche le message de demande XML qui est envoyé à partir du client sur le serveur lorsque vous utilisez l’opération [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="07180-129">The following example shows the XML request message that is sent from the client to the server when you use the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="07180-130">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [développer un groupe de distribution universel](#bk_ExpandDGEWSMA).</span><span class="sxs-lookup"><span data-stu-id="07180-130">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [expand a universal distribution group](#bk_ExpandDGEWSMA).</span></span> 
  
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

<span data-ttu-id="07180-131">L’exemple suivant affiche le message de réponse XML qui est envoyé à partir du serveur au client.</span><span class="sxs-lookup"><span data-stu-id="07180-131">The following example shows the XML response message that is sent from the server to the client.</span></span> <span data-ttu-id="07180-132">Notez que les boîtes aux lettres et des groupes de distribution universels sont retournés.</span><span class="sxs-lookup"><span data-stu-id="07180-132">Notice that both mailboxes and universal distribution groups are returned.</span></span>
  
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

<span data-ttu-id="07180-133">Contrairement à lorsque vous utilisez l’API managée EWS, lorsque vous utilisez EWS pour développer un groupe de distribution universel, vous ne pouvez pas de manière récursive développer les groupes de distribution sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="07180-133">Unlike when you use the EWS Managed API, when you use EWS to expand a universal distribution group, you can't recursively expand the distribution groups that are returned.</span></span> <span data-ttu-id="07180-134">Vous devez envoyer une demande supplémentaire afin de développer chacun des groupes de distribution inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="07180-134">You will need to send an additional request to expand each of the distribution groups included in the response.</span></span>
  
## <a name="expand-a-contact-group-by-using-ews"></a><span data-ttu-id="07180-135">Développez un groupe de contacts à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07180-135">Expand a contact group by using EWS</span></span>
<span data-ttu-id="07180-136"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="07180-136"></span></span>

<span data-ttu-id="07180-137">La demande XML pour développer un groupe de contacts est similaire à une demande pour développer un groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="07180-137">The XML request to expand a contact group is similar to a request to expand a distribution group.</span></span> <span data-ttu-id="07180-138">Au lieu d’une adresse de messagerie, vous utilisez l' [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de groupe de contacts.</span><span class="sxs-lookup"><span data-stu-id="07180-138">Instead of an email address, you use the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the contact group.</span></span> <span data-ttu-id="07180-139">L' **ID d’élément** dans cet exemple est réduite pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="07180-139">The **ItemId** in this example is shortened for readability.</span></span> 
  
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

<span data-ttu-id="07180-140">La structure de la réponse XML à une demande pour développer un groupe de contacts est la même que la réponse à une demande pour développer un groupe de distribution universel.</span><span class="sxs-lookup"><span data-stu-id="07180-140">The structure of the XML response to a request to expand a contact group is the same as the response to a request to expand a universal distribution group.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="07180-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07180-141">See also</span></span>


- [<span data-ttu-id="07180-142">Les groupes de distribution et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07180-142">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="07180-143">Créer des groupes de contacts à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07180-143">Create contact groups by using EWS in Exchange</span></span>](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

