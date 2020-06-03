---
title: Envoyer des messages électroniques à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 5290fafe-8b51-4275-a27e-baf497fc969c
description: Découvrez comment envoyer de nouveaux ou des brouillons de messages électroniques ou envoyer un message électronique différé à l’aide de l’API managée EWS ou EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: b73327cc69db37028c0508af788bf5294e79206a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527725"
---
# <a name="send-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="1f6fe-103">Envoyer des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1f6fe-103">Send email messages by using EWS in Exchange</span></span>

<span data-ttu-id="1f6fe-104">Découvrez comment envoyer de nouveaux ou des brouillons de messages électroniques ou envoyer un message électronique différé à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-104">Learn how to send new or draft email messages, or to send a delayed email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1f6fe-105">Que vous utilisiez l’API managée EWS ou EWS, vous pouvez envoyer des messages électroniques de deux manières.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-105">Whether you are using the EWS Managed API or EWS, you can send email messages in two ways.</span></span> <span data-ttu-id="1f6fe-106">Vous pouvez envoyer un message existant, tel qu’un message stocké dans votre dossier Brouillons, ou vous pouvez créer et envoyer un courrier électronique en une seule étape.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-106">You can either send an existing message, such as a message stored in your Drafts folder, or you can create and send an email in one step.</span></span> <span data-ttu-id="1f6fe-107">Les méthodes et les opérations que vous utilisez pour envoyer le message sont les mêmes, que vous envoyiez un message immédiatement ou que vous envoyiez un message différé.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-107">The methods and operations that you use to send the message are the same whether you're sending a message immediately, or sending a delayed message.</span></span>
  
<span data-ttu-id="1f6fe-108">**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour l’envoi de messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="1f6fe-108">**Table 1. EWS Managed API methods and EWS operations for sending email messages**</span></span>

|<span data-ttu-id="1f6fe-109">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="1f6fe-109">**Task**</span></span>|<span data-ttu-id="1f6fe-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="1f6fe-110">**EWS Managed API method**</span></span>|<span data-ttu-id="1f6fe-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="1f6fe-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1f6fe-112">Envoyer un nouveau message électronique</span><span class="sxs-lookup"><span data-stu-id="1f6fe-112">Send a new email message</span></span>  <br/> |[<span data-ttu-id="1f6fe-113">EmailMessage. Méthodesendandsavecopy</span><span class="sxs-lookup"><span data-stu-id="1f6fe-113">EmailMessage.SendAndSaveCopy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1f6fe-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="1f6fe-114">CreateItem</span></span>](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="1f6fe-115">Envoyer un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="1f6fe-115">Send an existing email message</span></span>  <br/> |[<span data-ttu-id="1f6fe-116">EmailMessage. Send</span><span class="sxs-lookup"><span data-stu-id="1f6fe-116">EmailMessage.Send</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1f6fe-117">SendItem</span><span class="sxs-lookup"><span data-stu-id="1f6fe-117">SendItem</span></span>](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> |
   
## <a name="send-a-new-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="1f6fe-118">Envoyer un nouveau message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-118">Send a new email message by using the EWS Managed API</span></span>
<span data-ttu-id="1f6fe-119"><a name="bk_sendnewewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-119"><a name="bk_sendnewewsma"> </a></span></span>

<span data-ttu-id="1f6fe-120">L’exemple de code suivant montre comment utiliser l’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique et la méthode [méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message au destinataire et l’enregistrer dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-120">The following code example shows how to use the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message and the [SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="1f6fe-121">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-121">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "' and saved in the SendItems folder.");
```

## <a name="send-a-new-email-message-by-using-ews"></a><span data-ttu-id="1f6fe-122">Envoyer un nouveau message électronique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-122">Send a new email message by using EWS</span></span>
<span data-ttu-id="1f6fe-123"><a name="bk_sendnewews"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-123"><a name="bk_sendnewews"> </a></span></span>

<span data-ttu-id="1f6fe-124">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec une valeur **MessageDisposition** de **méthodesendandsavecopy** pour créer un message électronique, envoyer le message au destinataire et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-124">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, send the message to the recipient, and save the message in the Sent Items folder.</span></span> <span data-ttu-id="1f6fe-125">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous [envoyez un nouveau message électronique](#bk_sendnewewsma).</span><span class="sxs-lookup"><span data-stu-id="1f6fe-125">This is also the XML request that the EWS Managed API sends when you [send a new email message](#bk_sendnewewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1f6fe-126">Le serveur répond à la demande**CreateItem** par un message [GetItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), qui inclut [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) renvoyant la valeur **NoError**, indiquant que le message a bien été créé, et où apparaît l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du nouveau message.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-126">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="send-a-draft-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="1f6fe-127">Envoyer un brouillon de message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-127">Send a draft email message by using the EWS Managed API</span></span>
<span data-ttu-id="1f6fe-128"><a name="bk_senddraftewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-128"><a name="bk_senddraftewsma"> </a></span></span>

<span data-ttu-id="1f6fe-129">L’exemple de code suivant montre comment envoyer un message qui a été stocké dans le dossier Brouillons, comme indiqué dans [créer un message électronique à l’aide de l’API managée EWS](email-and-ews-in-exchange.md#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="1f6fe-129">The following code example shows how to send a message that was stored in the Drafts folder, as shown in [Create an email message by using the EWS Managed API](email-and-ews-in-exchange.md#bk_createewsma).</span></span> <span data-ttu-id="1f6fe-130">Tout d’abord, utilisez la méthode [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour extraire le message, puis utilisez la méthode [Send](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) pour envoyer le message électronique, comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-130">First, use the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to retrieve the message, and then use the [Send](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to send the email message, as shown in the following code example.</span></span> <span data-ttu-id="1f6fe-131">Notez que cette méthode n’enregistre pas le message envoyé dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-131">Note that this method does not save the sent message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="1f6fe-132">Dans ce cas, les propriétés [EmailMessageSchema. Subject](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) et [EmailMessageSchema. ToRecipients](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) sont ajoutées à la propriété [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) de sorte que les valeurs puissent être incluses dans la sortie de la console.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-132">In this case, the [EmailMessageSchema.Subject](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) and [EmailMessageSchema.ToRecipients](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) properties are added to the [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) so that the values can be included in the console output.</span></span> 
  
<span data-ttu-id="1f6fe-133">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-133">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
// Send the email message.
// This method call results in a SendItem call to EWS.
message.Send();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "'.");
```

## <a name="send-a-draft-email-message-by-using-ews"></a><span data-ttu-id="1f6fe-134">Envoyer un brouillon de message électronique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-134">Send a draft email message by using EWS</span></span>
<span data-ttu-id="1f6fe-135"><a name="bk_senddraftews"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-135"><a name="bk_senddraftews"> </a></span></span>

<span data-ttu-id="1f6fe-136">Les exemples de code suivants montrent comment envoyer un message qui était stocké précédemment dans le dossier Brouillons, comme illustré dans la procédure [créer un message électronique à l’aide d’EWS](email-and-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="1f6fe-136">The following code examples show how to send a message that was previously stored in the Drafts folder, as shown in [Create an email message by using EWS](email-and-ews-in-exchange.md#bk_createews).</span></span> <span data-ttu-id="1f6fe-137">Utilisez d’abord l’opération [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer le message électronique à envoyer.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-137">First use the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to retrieve the email message to send.</span></span> <span data-ttu-id="1f6fe-138">Ensuite, utilisez l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) pour envoyer le message électronique aux destinataires et l’enregistrer dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-138">Then use the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the email message to recipients and save it in the Sent Items folder.</span></span> 
  
<span data-ttu-id="1f6fe-139">Le premier message, le message de demande **GetItem** , spécifie l' [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du brouillon de message électronique auquel se lier, et les éléments de l’élément [ItemShape](https://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) limitent les résultats à inclure dans la réponse **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="1f6fe-139">The first message, the **GetItem** request message, specifies the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the draft email message to bind to, and elements in the [ItemShape](https://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) element limit the results to include in the **GetItem** response.</span></span> <span data-ttu-id="1f6fe-140">L' **élément ItemShape** a un [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) de **IdOnly**, et l’élément [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) inclut les valeurs [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) de la propriété **Subject** du schéma d’élément et de la propriété **ToRecipients** du schéma de message, ce qui signifie que seuls les éléments **ItemId**, [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)et [ToRecipients](https://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) seront renvoyés au client dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-140">The **ItemShape** element has a [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) of **IdOnly**, and the [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element includes the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) values for the **Subject** property from the Item schema and the **ToRecipients** property from the Message schema, which means that only the **ItemId**, [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx), and [ToRecipients](https://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) elements will be returned to the client in the response.</span></span> <span data-ttu-id="1f6fe-141">Pour plus d’informations sur la limitation des valeurs renvoyées dans les appels et la signification de l’élément **BaseShape** , voir [Property sets and Response Shapes in EWS in Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="1f6fe-141">For more information about limiting the values returned in calls and the meaning of the **BaseShape** element, see [Property sets and response shapes in EWS in Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="1f6fe-142">Il s’agit également de la requête XML envoyée par l’API managée EWS lors de l’appel de la méthode [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1f6fe-142">This is also the XML request that is sent by the EWS Managed API when calling the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="1f6fe-143">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-143">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="message:ToRecipients" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADE4=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant présente la réponse XML que le serveur renvoie après avoir effectué l’opération **GetItem**. La réponse indique que le message électronique a été correctement récupéré et inclut les éléments **Subject** et **ToRecipient** comme demandé. <span data-ttu-id="1f6fe-146">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-146">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="842"
                         MinorBuildNumber="10"
                         Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAMkADE4="
                        ChangeKey="CQAAABYA" />
              <t:Subject>Project priorities</t:Subject>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>sadie@contoso.com</t:Name>
                  <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                  <t:MailboxType>OneOff</t:MailboxType>
                </t:Mailbox>
              </t:ToRecipients>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1f6fe-147">Le deuxième message, le message de demande **SendItem** , spécifie l' [ID ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique à envoyer, ainsi que le [SavedItemFolderId](https://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), qui spécifie le dossier dans lequel enregistrer l’élément envoyé.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-147">The second message, the **SendItem** request message, specifies the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to send, as well as the [SavedItemFolderId](https://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), which specifies the folder in which to save the sent item.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADE4="
                  ChangeKey="CQAAABYA" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1f6fe-148">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le courrier électronique a été envoyé avec succès.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-148">The server responds to the **SendItem** request with a [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="send-a-delayed-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="1f6fe-149">Envoyer un message électronique différé à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-149">Send a delayed email message by using the EWS Managed API</span></span>
<span data-ttu-id="1f6fe-150"><a name="bk_senddelayedewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-150"><a name="bk_senddelayedewsma"> </a></span></span>

<span data-ttu-id="1f6fe-151">L’exemple de code suivant montre comment utiliser l’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique, la classe [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) pour créer une définition de propriété pour la propriété [PidTagDeferredSendTime](https://msdn.microsoft.com/library/cc840017.aspx) (0x3FEF0040) et la méthode [méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer un message différé et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-151">The following code example shows how to use the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message, the [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) class to create a property definition for the [PidTagDeferredSendTime](https://msdn.microsoft.com/library/cc840017.aspx) (0x3FEF0040) property, and the [SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send a delayed message and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="1f6fe-152">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-152">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a new email message. 
EmailMessage message = new EmailMessage(service);
// Specify the email recipient and subject. 
message.ToRecipients.Add("sadie@contoso.com");
message.Subject = "Delayed email";
// Identify the extended property that can be used to specify when to send the email. 
ExtendedPropertyDefinition PidTagDeferredSendTime = new ExtendedPropertyDefinition(16367, MapiPropertyType.SystemTime);
// Set the time that will be used to specify when the email is sent. 
// In this example, the email will be sent one minute after the next line executes, 
// provided that the message.SendAndSaveCopy request is processed by the server within one minute. 
string sendTime = DateTime.Now.AddMinutes(1).ToUniversalTime().ToString();
// Specify when to send the email by setting the value of the extended property. 
message.SetExtendedProperty(PidTagDeferredSendTime, sendTime);
// Specify the email body. 
StringBuilder str = new StringBuilder();
str.AppendLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
str.AppendLine("The email message will be sent at: " + sendTime + ".");
message.Body = str.ToString();
Console.WriteLine("");
Console.WriteLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
Console.WriteLine("The email message will be sent at: " + sendTime + ".");
// Submit the request to send the email message. 
message.SendAndSaveCopy();
```

## <a name="send-a-delayed-email-message-by-using-ews"></a><span data-ttu-id="1f6fe-153">Envoyer un message électronique différé à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="1f6fe-153">Send a delayed email message by using EWS</span></span>
<span data-ttu-id="1f6fe-154"><a name="bk_senddelayedews"> </a></span><span class="sxs-lookup"><span data-stu-id="1f6fe-154"><a name="bk_senddelayedews"> </a></span></span>

<span data-ttu-id="1f6fe-155">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec une valeur **MessageDisposition** de **méthodesendandsavecopy** pour créer un message électronique, l’élément [ExtendedProperty](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) pour créer une définition de propriété pour la propriété [PidTagDeferredSendTime](https://msdn.microsoft.com/library/cc840017.aspx) (0x3FEF0040) afin de définir l’heure d’envoi du message et l’élément [SavedItemFolderId](https://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) pour enregistrer le message envoyé dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-155">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, the [ExtendedProperty](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) element to create a property definition for the [PidTagDeferredSendTime](https://msdn.microsoft.com/library/cc840017.aspx) (0x3FEF0040) property to set a time to send the message, and the [SavedItemFolderId](https://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) element to save the sent message in the Sent Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Delayed email</t:Subject>
          <t:Body BodyType="HTML">
            The client submitted the SendAndSaveCopy request at: 1/2/2014 9:08:52 PM.
            The email message will be sent at: 1/2/2014 9:09:52 PM.
          </t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI PropertyTag="16367"
                                PropertyType="SystemTime" />
            <t:Value>2014-01-02T21:09:52.000</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1f6fe-156">Le serveur répond à la demande**CreateItem** par un message [GetItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), qui inclut [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) renvoyant la valeur **NoError**, indiquant que le message a bien été créé, et où apparaît l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du nouveau message.</span><span class="sxs-lookup"><span data-stu-id="1f6fe-156">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1f6fe-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f6fe-157">See also</span></span>


- [<span data-ttu-id="1f6fe-158">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="1f6fe-158">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="1f6fe-159">Répondre à des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1f6fe-159">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    

