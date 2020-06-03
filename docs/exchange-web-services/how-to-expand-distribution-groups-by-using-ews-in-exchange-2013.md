---
title: Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Découvrez comment développer un groupe de distribution à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 2cbeb65b5a722bce4d5cab8fd716230874a6afca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528117"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a><span data-ttu-id="c4f0d-103">Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="c4f0d-103">Expand distribution groups by using EWS in Exchange 2013</span></span>

<span data-ttu-id="c4f0d-104">Découvrez comment développer un groupe de distribution à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-104">Learn how to expand a distribution group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="c4f0d-105">Vous pouvez utiliser la méthode de l’API managée EWS [ExchangeService. expandgroup,](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour développer un groupe de distribution afin d’identifier tous les destinataires.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-105">You can use the [ExchangeService.ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS operation to expand a distribution group to identify all recipients.</span></span> 
  
<span data-ttu-id="c4f0d-106">Étant donné que la méthode [expandgroup,](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) est surchargée, vous pouvez l’appeler de plusieurs façons :</span><span class="sxs-lookup"><span data-stu-id="c4f0d-106">Because the [ExpandGroup](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) method is overloaded, you can call it in several ways:</span></span> 
  
- <span data-ttu-id="c4f0d-107">[Expandgroup, (String)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx) -développe un groupe identifié par une adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-107">[ExpandGroup(String)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address.</span></span> 
    
- <span data-ttu-id="c4f0d-108">[Expandgroup, (EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) -développe un groupe identifié par une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-108">[ExpandGroup(EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) - Expands a group identified by an email address.</span></span> 
    
- <span data-ttu-id="c4f0d-109">[Expandgroup, (itemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) -développe un groupe identifié par un ID de groupe.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-109">[ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) - Expands a group identified by a group ID.</span></span> 
    
- <span data-ttu-id="c4f0d-110">[ExpanGroup (String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx) -développe un groupe identifié par une adresse SMTP et le type de routage de cette adresse.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-110">[ExpanGroup(String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address and the routing type of that address.</span></span> 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a><span data-ttu-id="c4f0d-111">Développer un groupe de distribution universel ou un groupe de sécurité à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c4f0d-111">Expand a universal distribution group or security group by using EWS Managed API</span></span>
<span data-ttu-id="c4f0d-112"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c4f0d-112"><a name="bk_ExpandDGEWSMA"> </a></span></span>

<span data-ttu-id="c4f0d-113">L’exemple suivant montre comment développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’une adresse de messagerie, qui est l’approche la plus simple.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-113">The following example shows how to expand a universal distribution group or security group by using an email address, which is the simplest approach.</span></span> <span data-ttu-id="c4f0d-114">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-114">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

<span data-ttu-id="c4f0d-115">Il ne s’agit pas d’une grande quantité de code, mais il s’agit également de la base de la recherche.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-115">That's not a lot of code, but it's also pretty basic and might not give you what you are looking for.</span></span> <span data-ttu-id="c4f0d-116">Nous allons donc aller plus en détail.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-116">So let's take it a step further.</span></span> <span data-ttu-id="c4f0d-117">Les groupes de distribution peuvent également contenir d’autres groupes de distribution.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-117">Distribution groups can also contain other distribution groups.</span></span> <span data-ttu-id="c4f0d-118">Il suffit de le développer pour générer l’adresse de messagerie des groupes de distribution contenus, mais pas de les développer.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-118">Simply expanding it will output the email address of the contained distribution groups but not expand them.</span></span> <span data-ttu-id="c4f0d-119">En ajoutant quelques lignes de code, vous pouvez développer de manière récursive les groupes pour afficher chaque contact.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-119">By adding a few more lines of code, you can recursively expand the groups to output every contact.</span></span>
  
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

<span data-ttu-id="c4f0d-120">À présent, vous pouvez appeler cette nouvelle fonction dans le code de votre code et développer tous les groupes de distribution publics contenus dans le premier.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-120">And now you can call this new function in the your code and expand all the public distribution groups contained within the first one.</span></span>
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a><span data-ttu-id="c4f0d-121">Développer un groupe de contacts à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c4f0d-121">Expand a contact group by using EWS Managed API</span></span>
<span data-ttu-id="c4f0d-122"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c4f0d-122"><a name="bk_ExpandDGEWSMA"> </a></span></span>

<span data-ttu-id="c4f0d-123">Étant donné que les groupes de contacts n’ont pas d’adresse de messagerie associée, vous devez développer le groupe en fonction de l’ItemId à l’aide de la méthode [expandgroup, (itemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c4f0d-123">Because contact groups do not have an associated email address, you need to expand the group based on the ItemId by using the [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="c4f0d-124">Vous pouvez créer une fonction, comme indiqué dans l’exemple précédent, et remplacer le deuxième type de paramètre de la chaîne par un [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c4f0d-124">You can create a function, as shown in the previous example, and change the second parameter type from a string to an [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span></span>
  
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

<span data-ttu-id="c4f0d-125">Vous pouvez désormais appeler cette fonction à l’aide de l’objet de service Exchange et de l' **ItemId** du groupe de contacts.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-125">Now you can call this function by using the Exchange service object and the **ItemId** of the contact group.</span></span> <span data-ttu-id="c4f0d-126">Notez que l' **ID ItemId** de l’exemple est raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-126">Note that the **ItemId** in the example is shortened for readability.</span></span> 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a><span data-ttu-id="c4f0d-127">Développer un groupe de distribution universel ou un groupe de sécurité à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="c4f0d-127">Expand a universal distribution group or security group by using EWS</span></span>
<span data-ttu-id="c4f0d-128"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c4f0d-128"><a name="bk_ExpandDGEWSMA"> </a></span></span>

<span data-ttu-id="c4f0d-129">L’exemple suivant montre le message de requête XML envoyé par le client au serveur lorsque vous utilisez l’opération [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c4f0d-129">The following example shows the XML request message that is sent from the client to the server when you use the [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="c4f0d-130">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [développer un groupe de distribution universel](#bk_ExpandDGEWSMA).</span><span class="sxs-lookup"><span data-stu-id="c4f0d-130">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [expand a universal distribution group](#bk_ExpandDGEWSMA).</span></span> 
  
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

<span data-ttu-id="c4f0d-131">L’exemple suivant montre le message de réponse XML envoyé par le serveur au client.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-131">The following example shows the XML response message that is sent from the server to the client.</span></span> <span data-ttu-id="c4f0d-132">Notez que les deux boîtes aux lettres et les groupes de distribution universels sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-132">Notice that both mailboxes and universal distribution groups are returned.</span></span>
  
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

<span data-ttu-id="c4f0d-133">Contrairement à l’API managée EWS, lorsque vous utilisez EWS pour développer un groupe de distribution universel, vous ne pouvez pas développer de manière récursive les groupes de distribution qui sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-133">Unlike when you use the EWS Managed API, when you use EWS to expand a universal distribution group, you can't recursively expand the distribution groups that are returned.</span></span> <span data-ttu-id="c4f0d-134">Vous devrez envoyer une demande supplémentaire pour développer chacun des groupes de distribution inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-134">You will need to send an additional request to expand each of the distribution groups included in the response.</span></span>
  
## <a name="expand-a-contact-group-by-using-ews"></a><span data-ttu-id="c4f0d-135">Développer un groupe de contacts à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="c4f0d-135">Expand a contact group by using EWS</span></span>
<span data-ttu-id="c4f0d-136"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c4f0d-136"><a name="bk_ExpandDGEWSMA"> </a></span></span>

<span data-ttu-id="c4f0d-137">La requête XML pour développer un groupe de contacts est semblable à une demande de développement d’un groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-137">The XML request to expand a contact group is similar to a request to expand a distribution group.</span></span> <span data-ttu-id="c4f0d-138">Au lieu d’une adresse de messagerie, vous utilisez l' [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du groupe de contacts.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-138">Instead of an email address, you use the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the contact group.</span></span> <span data-ttu-id="c4f0d-139">Dans cet exemple, l' **ItemId** est raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-139">The **ItemId** in this example is shortened for readability.</span></span> 
  
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

<span data-ttu-id="c4f0d-140">La structure de la réponse XML à une demande de développement d’un groupe de contacts est identique à la réponse à une demande de développement d’un groupe de distribution universel.</span><span class="sxs-lookup"><span data-stu-id="c4f0d-140">The structure of the XML response to a request to expand a contact group is the same as the response to a request to expand a universal distribution group.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c4f0d-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4f0d-141">See also</span></span>


- [<span data-ttu-id="c4f0d-142">Les groupes de distribution et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4f0d-142">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="c4f0d-143">Créer des groupes de contacts à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4f0d-143">Create contact groups by using EWS in Exchange</span></span>](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

