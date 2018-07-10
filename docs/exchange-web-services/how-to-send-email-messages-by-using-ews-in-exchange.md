---
title: Envoyer des messages électroniques à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 5290fafe-8b51-4275-a27e-baf497fc969c
description: Apprenez à envoyer des messages électroniques de nouveau ou un projet, ou pour envoyer un message électronique différée à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: f09babfcc420d4cbc563ed6605ba555fd9f8c7e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754934"
---
# <a name="send-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="b3dea-103">Envoyer des messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3dea-103">Send email messages by using EWS in Exchange</span></span>

<span data-ttu-id="b3dea-104">Apprenez à envoyer des messages électroniques de nouveau ou un projet, ou pour envoyer un message électronique différée à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3dea-104">Learn how to send new or draft email messages, or to send a delayed email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b3dea-105">Si vous utilisez les API managées EWS, vous pouvez envoyer des messages électroniques de deux manières.</span><span class="sxs-lookup"><span data-stu-id="b3dea-105">Whether you are using the EWS Managed API or EWS, you can send email messages in two ways.</span></span> <span data-ttu-id="b3dea-106">Vous pouvez envoyer un message existant, par exemple un message stocké dans le dossier Brouillons, ou vous pouvez créer et envoyer un message électronique en une seule étape.</span><span class="sxs-lookup"><span data-stu-id="b3dea-106">You can either send an existing message, such as a message stored in your Drafts folder, or you can create and send an email in one step.</span></span> <span data-ttu-id="b3dea-107">Les méthodes et les opérations que vous utilisez pour envoyer le message sont les mêmes que vous envoyez un message immédiatement, ou l’envoi d’un message différé.</span><span class="sxs-lookup"><span data-stu-id="b3dea-107">The methods and operations that you use to send the message are the same whether you're sending a message immediately, or sending a delayed message.</span></span>
  
<span data-ttu-id="b3dea-108">**Le tableau 1. Méthodes d’API managées et opérations EWS pour l’envoi de messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="b3dea-108">**Table 1. EWS Managed API methods and EWS operations for sending email messages**</span></span>

|<span data-ttu-id="b3dea-109">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="b3dea-109">**Task**</span></span>|<span data-ttu-id="b3dea-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="b3dea-110">**EWS Managed API method**</span></span>|<span data-ttu-id="b3dea-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="b3dea-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b3dea-112">Envoyer un message électronique</span><span class="sxs-lookup"><span data-stu-id="b3dea-112">Send a new email message</span></span>  <br/> |[<span data-ttu-id="b3dea-113">EmailMessage.SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="b3dea-113">EmailMessage.SendAndSaveCopy</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b3dea-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="b3dea-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="b3dea-115">Envoyer un message électronique existant</span><span class="sxs-lookup"><span data-stu-id="b3dea-115">Send an existing email message</span></span>  <br/> |[<span data-ttu-id="b3dea-116">EmailMessage.Send</span><span class="sxs-lookup"><span data-stu-id="b3dea-116">EmailMessage.Send</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b3dea-117">SendItem</span><span class="sxs-lookup"><span data-stu-id="b3dea-117">SendItem</span></span>](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> |
   
## <a name="send-a-new-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="b3dea-118">Envoyer un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-118">Send a new email message by using the EWS Managed API</span></span>
<span data-ttu-id="b3dea-119"><a name="bk_sendnewewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-119"></span></span>

<span data-ttu-id="b3dea-120">L’exemple de code suivant montre comment utiliser l’objet [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique et la méthode [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer le message au destinataire et enregistrez le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-120">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message and the [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="b3dea-121">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3dea-121">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="send-a-new-email-message-by-using-ews"></a><span data-ttu-id="b3dea-122">Envoyer un message électronique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-122">Send a new email message by using EWS</span></span>
<span data-ttu-id="b3dea-123"><a name="bk_sendnewews"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-123"></span></span>

<span data-ttu-id="b3dea-124">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec la valeur **MessageDisposition** **SendAndSaveCopy** pour créer un message électronique, envoyer le message au destinataire et enregistrez le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-124">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, send the message to the recipient, and save the message in the Sent Items folder.</span></span> <span data-ttu-id="b3dea-125">C’est également la demande XML que l’API managée EWS envoie lorsque vous [envoyez un message électronique](#bk_sendnewewsma).</span><span class="sxs-lookup"><span data-stu-id="b3dea-125">This is also the XML request that the EWS Managed API sends when you [send a new email message](#bk_sendnewewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b3dea-126">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé.</span><span class="sxs-lookup"><span data-stu-id="b3dea-126">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="send-a-draft-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="b3dea-127">Envoyer un message électronique de brouillon à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-127">Send a draft email message by using the EWS Managed API</span></span>
<span data-ttu-id="b3dea-128"><a name="bk_senddraftewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-128"></span></span>

<span data-ttu-id="b3dea-129">L’exemple de code suivant montre comment envoyer un message qui a été stocké dans le dossier Brouillons, comme indiqué dans [créer un message électronique à l’aide de l’API managée EWS](email-and-ews-in-exchange.md#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="b3dea-129">The following code example shows how to send a message that was stored in the Drafts folder, as shown in [Create an email message by using the EWS Managed API](email-and-ews-in-exchange.md#bk_createewsma).</span></span> <span data-ttu-id="b3dea-130">Tout d’abord, utilisez la méthode [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) pour récupérer le message, puis utilisez la méthode [Send](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) pour envoyer le message électronique, comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="b3dea-130">First, use the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to retrieve the message, and then use the [Send](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to send the email message, as shown in the following code example.</span></span> <span data-ttu-id="b3dea-131">Notez que cette méthode n’enregistre pas le message envoyé dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-131">Note that this method does not save the sent message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="b3dea-132">Dans ce cas, les propriétés [EmailMessageSchema.Subject](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) et [EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) sont ajoutées à la [classe PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) afin que les valeurs peuvent être inclus dans la sortie de la console.</span><span class="sxs-lookup"><span data-stu-id="b3dea-132">In this case, the [EmailMessageSchema.Subject](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) and [EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) properties are added to the [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) so that the values can be included in the console output.</span></span> 
  
<span data-ttu-id="b3dea-133">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3dea-133">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="send-a-draft-email-message-by-using-ews"></a><span data-ttu-id="b3dea-134">Envoyer un message électronique de brouillon à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-134">Send a draft email message by using EWS</span></span>
<span data-ttu-id="b3dea-135"><a name="bk_senddraftews"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-135"></span></span>

<span data-ttu-id="b3dea-136">Les exemples de code suivants montrent comment envoyer un message qui a été précédemment stocké dans le dossier Brouillons, comme indiqué dans [créer un message électronique à l’aide de EWS](email-and-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="b3dea-136">The following code examples show how to send a message that was previously stored in the Drafts folder, as shown in [Create an email message by using EWS](email-and-ews-in-exchange.md#bk_createews).</span></span> <span data-ttu-id="b3dea-137">Commencez par utiliser l’opération [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) pour récupérer le message électronique à envoyer.</span><span class="sxs-lookup"><span data-stu-id="b3dea-137">First use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to retrieve the email message to send.</span></span> <span data-ttu-id="b3dea-138">Utilisez ensuite l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) pour envoyer le message électronique aux destinataires et enregistrez-le dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-138">Then use the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the email message to recipients and save it in the Sent Items folder.</span></span> 
  
<span data-ttu-id="b3dea-139">Le premier message, le message de demande **GetItem** , spécifie l' [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique brouillon à lier et éléments dans l’élément [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) limiter les résultats à inclure dans la réponse **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="b3dea-139">The first message, the **GetItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the draft email message to bind to, and elements in the [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) element limit the results to include in the **GetItem** response.</span></span> <span data-ttu-id="b3dea-140">L’élément **ItemShape** a un [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) de **IdOnly**, et l’élément [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) inclut les valeurs [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) pour la propriété **Subject** dans le schéma de l’élément et le **ToRecipients** propriété à partir du schéma du Message, ce qui signifie que seuls les éléments **ItemId**, [l’objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)et [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) seront afficheront au client dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b3dea-140">The **ItemShape** element has a [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) of **IdOnly**, and the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element includes the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) values for the **Subject** property from the Item schema and the **ToRecipients** property from the Message schema, which means that only the **ItemId**, [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx), and [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) elements will be returned to the client in the response.</span></span> <span data-ttu-id="b3dea-141">Pour plus d’informations sur la limitation des valeurs renvoyées dans les appels et la signification de l’élément **BaseShape** , consultez la rubrique [jeux de propriétés et de réponse des formes dans EWS dans Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b3dea-141">For more information about limiting the values returned in calls and the meaning of the **BaseShape** element, see [Property sets and response shapes in EWS in Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="b3dea-142">C’est également la demande XML qui est envoyée par l’API managée EWS lors de l’appel de la méthode [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b3dea-142">This is also the XML request that is sent by the EWS Managed API when calling the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="b3dea-143">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b3dea-143">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

L’exemple suivant montre la réponse XML que le serveur renvoie une fois qu’il traite l’opération **GetItem** . La réponse indique que le message électronique a été récupéré avec succès et inclut les éléments de **l’objet** et **ToRecipient** comme requis. <span data-ttu-id="b3dea-146">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b3dea-146">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="842"
                         MinorBuildNumber="10"
                         Version="V2_8"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b3dea-147">Le deuxième message, le message de demande **SendItem** , spécifie l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du message électronique à envoyer, ainsi que la [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), qui spécifie le dossier dans lequel enregistrer l’élément envoyé.</span><span class="sxs-lookup"><span data-stu-id="b3dea-147">The second message, the **SendItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to send, as well as the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), which specifies the folder in which to save the sent item.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b3dea-148">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été envoyé correctement.</span><span class="sxs-lookup"><span data-stu-id="b3dea-148">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="send-a-delayed-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="b3dea-149">Envoyer un message électronique différée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-149">Send a delayed email message by using the EWS Managed API</span></span>
<span data-ttu-id="b3dea-150"><a name="bk_senddelayedewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-150"></span></span>

<span data-ttu-id="b3dea-151">L’exemple de code suivant montre comment utiliser l’objet [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) pour créer un message électronique, la classe [ExtendedPropertyDefinition](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) pour créer une définition de propriété pour la propriété [PidTagDeferredSendTime](http://msdn.microsoft.com/fr-fr/library/cc840017.aspx) (0x3FEF0040) et Méthode [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) pour envoyer un message différé et enregistrer le message dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-151">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message, the [ExtendedPropertyDefinition](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) class to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/fr-fr/library/cc840017.aspx) (0x3FEF0040) property, and the [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send a delayed message and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="b3dea-152">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3dea-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="send-a-delayed-email-message-by-using-ews"></a><span data-ttu-id="b3dea-153">Envoyer un message électronique différée à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b3dea-153">Send a delayed email message by using EWS</span></span>
<span data-ttu-id="b3dea-154"><a name="bk_senddelayedews"> </a></span><span class="sxs-lookup"><span data-stu-id="b3dea-154"></span></span>

<span data-ttu-id="b3dea-155">L’exemple de code suivant montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec la valeur **MessageDisposition** **SendAndSaveCopy** pour créer un message électronique, l’élément [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) pour créer une définition de propriété pour la [ PidTagDeferredSendTime](http://msdn.microsoft.com/fr-fr/library/cc840017.aspx) propriété (0x3FEF0040) pour définir une heure d’envoi du message, ainsi que l’élément [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) pour enregistrer le message envoyé dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b3dea-155">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, the [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) element to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/fr-fr/library/cc840017.aspx) (0x3FEF0040) property to set a time to send the message, and the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) element to save the sent message in the Sent Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b3dea-156">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé.</span><span class="sxs-lookup"><span data-stu-id="b3dea-156">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b3dea-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3dea-157">See also</span></span>


- [<span data-ttu-id="b3dea-158">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="b3dea-158">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b3dea-159">Répondre aux messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3dea-159">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    

