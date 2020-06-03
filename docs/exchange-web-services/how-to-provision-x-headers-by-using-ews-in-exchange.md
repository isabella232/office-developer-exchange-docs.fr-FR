---
title: Mise en service des en-têtes x à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 409ddb944bbac7a60242de39cdf7ae13b17cc76a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527767"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a><span data-ttu-id="5d91d-103">Mise en service des en-têtes x à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5d91d-103">Provision x-headers by using EWS in Exchange</span></span>

<span data-ttu-id="5d91d-104">Découvrez comment mettre en service des en-têtes x pour une boîte aux lettres à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d91d-104">Learn how to provision x-headers for a mailbox by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5d91d-105">Les en-têtes X sont des en-têtes non standard ajoutés à la collection d’en-têtes d’un message électronique pour communiquer des informations.</span><span class="sxs-lookup"><span data-stu-id="5d91d-105">X-headers are non-standard headers that are added to the header collection of an email to communicate information.</span></span> <span data-ttu-id="5d91d-106">Par exemple, Exchange marque les messages à l’aide de l’en-tête **X-MS-Exchange-Organization-SCL** pour indiquer le seuil de probabilité de courrier indésirable (SCL) attribué au courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="5d91d-106">For example, Exchange stamps messages with the **X-MS-Exchange-Organization-SCL** header to indicate the spam confidence level (SCL) attributed to the email.</span></span> <span data-ttu-id="5d91d-107">Les clients de messagerie comme Outlook peuvent utiliser ces informations pour déterminer le type d’action à effectuer sur le courrier électronique (par exemple, Outlook peut empêcher les images de s’afficher sauf si l’utilisateur effectue une action).</span><span class="sxs-lookup"><span data-stu-id="5d91d-107">Email clients like Outlook can use that information to determine what type of action to take on the email (for example, Outlook can prevent images from displaying unless the user takes an action).</span></span> 
  
<span data-ttu-id="5d91d-108">Exchange ajoute des en-têtes x entrants au schéma de boîte aux lettres en tant que propriété nommée la première fois qu’il reçoit un message électronique avec cet en-tête x.</span><span class="sxs-lookup"><span data-stu-id="5d91d-108">Exchange adds incoming x-headers to the mailbox schema as a named property the first time it receives an email with that x-header.</span></span> <span data-ttu-id="5d91d-109">La valeur de l’en-tête x n’est pas enregistrée dans le premier message électronique ; Toutefois, il est enregistré sur tous les messages électroniques suivants qui incluent l’en-tête x.</span><span class="sxs-lookup"><span data-stu-id="5d91d-109">The x-header value is not saved on that first email; however, it is saved on all subsequent emails that include the x-header.</span></span> <span data-ttu-id="5d91d-110">Pour cette raison, votre application doit mettre en service les en-têtes x avant de les utiliser.</span><span class="sxs-lookup"><span data-stu-id="5d91d-110">For this reason, your application should provision x-headers before you expect to use them.</span></span> <span data-ttu-id="5d91d-111">Le mappage entre une propriété nommée et un en-tête x se produit dans la remise du courrier électronique à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5d91d-111">The mapping between a named property and an x-header occurs in the transport delivery of the email to the mailbox.</span></span> <span data-ttu-id="5d91d-112">Cela signifie que vous devez recevoir le courrier électronique via la remise du transport ; vous ne pouvez pas simplement enregistrer un message électronique qui inclut l’en-tête x dans une boîte aux lettres pour créer le mappage à une propriété nommée.</span><span class="sxs-lookup"><span data-stu-id="5d91d-112">This means that you need to receive the email via transport delivery; you cannot just save an email that includes the x-header to a mailbox to create the mapping to a named property.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5d91d-113">Si vous constatez que les en-têtes x ne sont pas enregistrés, déterminez si un [agent de transport](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou un [pare-feu d’en-tête](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) filtre les en-têtes x avant qu’ils accèdent à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5d91d-113">If you find that x-headers aren't being saved, determine whether a [transport agent](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) or [header firewall](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) is filtering out your x-headers before they get to the mailbox.</span></span> <span data-ttu-id="5d91d-114">r</span><span class="sxs-lookup"><span data-stu-id="5d91d-114">r</span></span>
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a><span data-ttu-id="5d91d-115">Approvisionner un en-tête x à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5d91d-115">Provision an x-header by using the EWS Managed API</span></span>
<span data-ttu-id="5d91d-116"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="5d91d-116"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="5d91d-117">L’exemple de code suivant montre comment utiliser la méthode [EmailMessage. Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) de l’API managée EWS pour mettre en service un en-tête x pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5d91d-117">The following code example shows how to use the EWS Managed API [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to provision an x-header for a mailbox.</span></span> <span data-ttu-id="5d91d-118">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que la boîte aux lettres cible n’a pas dépassé le [quota pour les propriétés nommées](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5d91d-118">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the target mailbox hasn't exceeded the [quota for named properties](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span></span>
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a><span data-ttu-id="5d91d-119">Approvisionner un en-tête x à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="5d91d-119">Provision an x-header by using EWS</span></span>
<span data-ttu-id="5d91d-120"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="5d91d-120"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="5d91d-121">L’exemple de code suivant montre comment utiliser l’opération [CREATEITEM](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer et envoyer un message électronique pour approvisionner une boîte aux lettres avec un en-tête x.</span><span class="sxs-lookup"><span data-stu-id="5d91d-121">The following code example shows how to use the EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) operation to create and send an email to provision a mailbox with an x-header.</span></span> <span data-ttu-id="5d91d-122">Il s’agit de la requête XML envoyée par l’API managée EWS lorsque vous configurez [un en-tête x à l’aide de l’API managée EWS](#bk_example1).</span><span class="sxs-lookup"><span data-stu-id="5d91d-122">This is the XML request that is sent by the EWS Managed API when you [Provision an x-header by using the EWS Managed API](#bk_example1).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a><span data-ttu-id="5d91d-123">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="5d91d-123">Version differences</span></span>
<span data-ttu-id="5d91d-124"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="5d91d-124"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="5d91d-125">La première fois que vous approvisionnez un en-tête x dans Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’une version locale d’Exchange à partir d’Exchange Server 2010, la valeur d’un nouvel en-tête x personnalisé n’est pas écrite dans le message stocké.</span><span class="sxs-lookup"><span data-stu-id="5d91d-125">The first time that you provision an x-header in Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2010, the value of a new custom x-header will not be written to the stored message.</span></span> <span data-ttu-id="5d91d-126">Cela est dû au fait que l’en-tête x doit d’abord être mappé à une propriété nommée dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5d91d-126">This is because the x-header must first be mapped to a named property in the user's mailbox.</span></span> <span data-ttu-id="5d91d-127">Le mappage se produit lors de la première demande d’ajout des propriétés nommées.</span><span class="sxs-lookup"><span data-stu-id="5d91d-127">The mapping occurs upon the first request to add the named properties.</span></span> <span data-ttu-id="5d91d-128">Lorsqu’une demande ultérieure de création de la propriété nommée se produit, la propriété et la valeur sont stockées dans le message.</span><span class="sxs-lookup"><span data-stu-id="5d91d-128">When a subsequent request to create the named property occurs, the property and value are stored on the message.</span></span> <span data-ttu-id="5d91d-129">Dans Exchange 2007, la première fois qu’un en-tête x est écrit dans une base de données de boîtes aux lettres, un mappage est créé pour l’en-tête x vers une propriété nommée dans la base de données de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5d91d-129">In Exchange 2007, the first time an x-header is written to a mailbox database, a mapping is created for the x-header to a named property across the mailbox database.</span></span> <span data-ttu-id="5d91d-130">Lorsqu’une demande ultérieure de création de la propriété nommée se produit, l’en-tête x est traité et stocké pour toutes les boîtes aux lettres de la base de données Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="5d91d-130">When a subsequent request to create the named property occurs, the x-header is processed and stored for any mailbox in the Exchange 2007 database.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="5d91d-131">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="5d91d-131">Next steps</span></span>
<span data-ttu-id="5d91d-132"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="5d91d-132"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="5d91d-133">Cet article vous explique comment mettre en service un en-tête x pour une seule boîte aux lettres en envoyant un message électronique à un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5d91d-133">This article shows you how to provision an x-header for a single mailbox by sending an email to a user.</span></span> <span data-ttu-id="5d91d-134">Vous pouvez également configurer un en-tête x pour de nombreux utilisateurs en [envoyant un message électronique à une liste de destinataires](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) dans l’organisation de l’appelant.</span><span class="sxs-lookup"><span data-stu-id="5d91d-134">You can also provision an x-header for many users by [sending a batch email to a list of recipients](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) in the caller's organization.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5d91d-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5d91d-135">See also</span></span>


- [<span data-ttu-id="5d91d-136">Les propriétés et les propriétés étendues dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5d91d-136">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="5d91d-137">Exchange 2013 : mise en service des en-têtes X personnalisés par programme</span><span class="sxs-lookup"><span data-stu-id="5d91d-137">Exchange 2013: Provision custom X-headers programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [<span data-ttu-id="5d91d-138">Propriétés nommées, en-têtes X et vous</span><span class="sxs-lookup"><span data-stu-id="5d91d-138">Named Properties, X-Headers, and You</span></span>](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [<span data-ttu-id="5d91d-139">Propriétés nommées, rond 2 : ce qui est en avance</span><span class="sxs-lookup"><span data-stu-id="5d91d-139">Named Properties, Round 2: What lies Ahead</span></span>](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [<span data-ttu-id="5d91d-140">Pare-feu d’en-tête</span><span class="sxs-lookup"><span data-stu-id="5d91d-140">Header Firewall</span></span>](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="5d91d-141">EWS, MIME et les en-têtes de message Internet manquants</span><span class="sxs-lookup"><span data-stu-id="5d91d-141">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [<span data-ttu-id="5d91d-142">Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5d91d-142">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

