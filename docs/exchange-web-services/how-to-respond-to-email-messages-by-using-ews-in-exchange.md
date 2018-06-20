---
title: Répondre aux messages électroniques à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d584991-4d67-4d36-ae2f-99970af8488f
description: Découvrez comment répondre aux messages électroniques à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 2f1428251084a7f2bf8d589a788c143f34b64d5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754936"
---
# <a name="respond-to-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="6f46b-103">Répondre aux messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6f46b-103">Respond to email messages by using EWS in Exchange</span></span>

<span data-ttu-id="6f46b-104">Découvrez comment répondre aux messages électroniques à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f46b-104">Learn how to respond to email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6f46b-105">Vous pouvez utiliser les API managées EWS pour répondre aux messages en réponse à leur ou les transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="6f46b-105">You can use the EWS Managed API or EWS to respond to messages by replying to them or forwarding them to recipients.</span></span>
  
<span data-ttu-id="6f46b-106">**Le tableau 1. Méthodes d’API managées et opérations EWS pour répondre aux messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="6f46b-106">**Table 1. EWS Managed API methods and EWS operations for responding to email messages**</span></span>

|<span data-ttu-id="6f46b-107">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="6f46b-107">**Task**</span></span>|<span data-ttu-id="6f46b-108">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="6f46b-108">**EWS Managed API method**</span></span>|<span data-ttu-id="6f46b-109">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="6f46b-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6f46b-110">Répondre à un message électronique</span><span class="sxs-lookup"><span data-stu-id="6f46b-110">Reply to an email message</span></span>  <br/> |[<span data-ttu-id="6f46b-111">EmailMessage.Reply</span><span class="sxs-lookup"><span data-stu-id="6f46b-111">EmailMessage.Reply</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="6f46b-112">EmailMessage.CreateReply</span><span class="sxs-lookup"><span data-stu-id="6f46b-112">EmailMessage.CreateReply</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6f46b-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), en où l’élément [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) a un élément enfant de [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) ou [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6f46b-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of either [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) or [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="6f46b-114">Transférer un message électronique</span><span class="sxs-lookup"><span data-stu-id="6f46b-114">Forward an email message</span></span>  <br/> |[<span data-ttu-id="6f46b-115">EmailMessage.Forward</span><span class="sxs-lookup"><span data-stu-id="6f46b-115">EmailMessage.Forward</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="6f46b-116">EmailMessage.CreateForward</span><span class="sxs-lookup"><span data-stu-id="6f46b-116">EmailMessage.CreateForward</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="6f46b-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), en où l’élément [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) a un élément enfant de [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6f46b-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span></span>  <br/> |
   
## <a name="reply-to-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="6f46b-118">Répondre à un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6f46b-118">Reply to an email message by using the EWS Managed API</span></span>
<span data-ttu-id="6f46b-119"><a name="bk_replyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6f46b-119"></span></span>

<span data-ttu-id="6f46b-120">L’API managée EWS fournit deux méthodes que vous pouvez utiliser pour répondre aux messages : [réponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) et [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6f46b-120">The EWS Managed API provides two methods that you can use to respond to messages: [Reply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) and [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="6f46b-121">La méthode **Reply** ne prend deux paramètres : le message de réponse pour faire précéder le corps existant et une valeur de **type Boolean** qui indique si la réponse doit atteindre tous les destinataires (true) ou uniquement l’expéditeur (false).</span><span class="sxs-lookup"><span data-stu-id="6f46b-121">The **Reply** method only takes two parameters: the response message to prepend to the existing body, and a **Boolean** value that indicates whether the response should go to all recipients (true) or just the sender (false).</span></span> <span data-ttu-id="6f46b-122">Si vous avez besoin pour ajouter des destinataires à un message, définir des propriétés supplémentaires sur une réponse, ou ajouter une pièce jointe, utilisez la méthode **CreateReply** , qui permet de définir toutes les [Propriétés de première classe](email-properties-and-elements-in-ews-in-exchange.md) qui sont disponibles sur un [EmailMessage ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)objet.</span><span class="sxs-lookup"><span data-stu-id="6f46b-122">If you need to add additional recipients to a message, set additional properties on a response, or add an attachment, use the **CreateReply** method, which enables you to set all the [first-class properties](email-properties-and-elements-in-ews-in-exchange.md) that are available on an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="6f46b-123">L’exemple de code suivant montre comment utiliser la méthode **Reply** pour répondre à un message électronique.</span><span class="sxs-lookup"><span data-stu-id="6f46b-123">The following code example shows how to use the **Reply** method to respond to an email message.</span></span> 
  
<span data-ttu-id="6f46b-124">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f46b-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="6f46b-125">La variable locale *ItemId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément pour répondre à.</span><span class="sxs-lookup"><span data-stu-id="6f46b-125">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to respond to.</span></span> <span data-ttu-id="6f46b-126">L’exemple appelle la [méthode FindRecentlySent](#bk_findlast) pour vérifier que le message a été marqué comme une réponse.</span><span class="sxs-lookup"><span data-stu-id="6f46b-126">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as replied to.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.LastModifiedTime);
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
string myReply = "This is the message body of the email reply.";
bool replyToAll = false;
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Reply(myReply, replyToAll);
// Verify that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="6f46b-127">L’exemple de code suivant montre comment utiliser la méthode **CreateReply** pour répondre à un message électronique.</span><span class="sxs-lookup"><span data-stu-id="6f46b-127">The following code example shows how to use the **CreateReply** method to respond to an email message.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
bool replyToAll = true;
ResponseMessage responseMessage = message.CreateReply(replyToAll);
// Prepend the reply to the message body. 
string myReply = "This is the message body of the email reply.";
responseMessage.BodyPrefix = myReply;
// Send the response message.
// This method call results in a CreateItem call to EWS.
responseMessage.SendAndSaveCopy();
// Check that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="6f46b-128">Si vous souhaitez ajouter une pièce jointe au message de réponse, remplacez l’appel à la méthode **SendAndSaveCopy** par le code suivant.</span><span class="sxs-lookup"><span data-stu-id="6f46b-128">If you need to add an attachment to the response message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage reply = responseMessage.Save();
reply.Attachments.AddFileAttachment("attachmentname.txt");
reply.Update(ConflictResolutionMode.AutoResolve);
reply.SendAndSaveCopy();
```

## <a name="reply-to-an-email-message-by-using-ews"></a><span data-ttu-id="6f46b-129">Répondre à un message électronique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="6f46b-129">Reply to an email message by using EWS</span></span>
<span data-ttu-id="6f46b-130"><a name="bk_replyews"> </a></span><span class="sxs-lookup"><span data-stu-id="6f46b-130"></span></span>

<span data-ttu-id="6f46b-131">L’exemple de code suivant montre comment répondre à un message à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="6f46b-131">The following code example shows how to reply to a message by using EWS.</span></span> <span data-ttu-id="6f46b-132">Utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec l’attribut **MessageDisposition** **SendAndSaveCopy** pour envoyer le message et enregistrez la réponse dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="6f46b-132">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="6f46b-133">Inclure soit l’élément [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) en tant qu’enfant de l’élément [éléments](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) répondre à tout le monde sur le thread de message, ou inclure l’élément [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) pour répondre uniquement à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="6f46b-133">Include either the [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) element as a child of the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element to reply to everyone on the message thread, or include the [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) element to reply only to the sender.</span></span> 
  
<span data-ttu-id="6f46b-134">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) soit la [réponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6f46b-134">This is also the XML request that the EWS Managed API sends when calling either the [Reply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) or the [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ReplyAllToItem>
          <t:ReferenceItemId Id="AAMkADE4="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the email reply.</t:NewBodyContent>
        </t:ReplyAllToItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f46b-135">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la réponse a été créée et envoyée avec succès.</span><span class="sxs-lookup"><span data-stu-id="6f46b-135">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the reply was created and sent successfully.</span></span>
  
<span data-ttu-id="6f46b-136">Si vous souhaitez ajouter une pièce jointe à votre message de réponse, appelez l’opération **CreateItem** comme indiqué ci-dessus, mais remplacez le **MessageDisposition** **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="6f46b-136">If you need to add an attachment to your response message, call the **CreateItem** operation as specified above, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="6f46b-137">Appelez ensuite l’opération [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , suivie de l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6f46b-137">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="forward-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="6f46b-138">Transférer un message électronique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6f46b-138">Forward an email message by using the EWS Managed API</span></span>
<span data-ttu-id="6f46b-139"><a name="bk_forwardewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6f46b-139"></span></span>

<span data-ttu-id="6f46b-140">L’API managée EWS fournit deux méthodes que vous pouvez utiliser pour transférer les messages : [vers le bas](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) et [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6f46b-140">The EWS Managed API provides two methods that you can use to forward messages: [Forward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) and [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="6f46b-141">La méthode **Forward** n’accepte que les deux paramètres : le message pour faire précéder le corps existant et un tableau ou une collection de destinataires, en fonction de la surcharge que vous choisissez d’utiliser.</span><span class="sxs-lookup"><span data-stu-id="6f46b-141">The **Forward** method only takes two parameters: the message to prepend to the existing body, and an array or collection of recipients, depending on the overload you choose to use.</span></span> <span data-ttu-id="6f46b-142">Si vous souhaitez ajouter une pièce jointe au message vous transfert, ou définissez des propriétés supplémentaires sur le nouveau message, utilisez la méthode **CreateForward** , qui permet de définir toutes les propriétés qui sont disponibles sur un objet [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6f46b-142">If you need to add an attachment to the message you're forwarding, or set additional properties on the new message, use the **CreateForward** method, which enables you to set all the properties that are available on an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="6f46b-143">L’exemple de code suivant montre comment utiliser la méthode **Forward** pour transférer un message électronique à un destinataire.</span><span class="sxs-lookup"><span data-stu-id="6f46b-143">The following code example shows how to use the **Forward** method to forward an email message to one recipient.</span></span> 
  
<span data-ttu-id="6f46b-144">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f46b-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="6f46b-145">La variable locale *ItemId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à transférer.</span><span class="sxs-lookup"><span data-stu-id="6f46b-145">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to forward.</span></span> <span data-ttu-id="6f46b-146">L’exemple appelle la [méthode FindRecentlySent](#bk_findlast) pour vérifier que le message a été marqué comme transféré.</span><span class="sxs-lookup"><span data-stu-id="6f46b-146">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as forwarded.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
string myForward = "This is the message body of the forwarded email.";
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Forward(myForward, "sadie@contoso.com");
// Verify that the forwarded response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="6f46b-147">L’exemple de code suivant montre comment utiliser la méthode **CreateForward** pour transférer un message électronique à un destinataire.</span><span class="sxs-lookup"><span data-stu-id="6f46b-147">The following code example shows how to use the **CreateForward** method to forward an email message to one recipient.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
ResponseMessage forwardMessage = message.CreateForward();
// Set properties on the email message.
forwardMessage.ToRecipients.Add("sadie@contoso.com");
forwardMessage.Body = "Sadie,<br><br>I thought you'd be interested in this thread.<br><br>-Mack";
// Send and save a copy of the replied email message in the default Sent Items folder. 
forwardMessage.SendAndSaveCopy();
// Verify that the forwarded message was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="6f46b-148">Si vous souhaitez ajouter une pièce jointe au message transmis, remplacez l’appel à la méthode **SendAndSaveCopy** par le code suivant.</span><span class="sxs-lookup"><span data-stu-id="6f46b-148">If you need to add an attachment to the forwarded message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage forward = forwardMessage.Save();
forward.Attachments.AddFileAttachment("attachmentname.txt");
forward.Update(ConflictResolutionMode.AutoResolve);
forward.SendAndSaveCopy();
```

## <a name="forward-an-email-message-by-using-ews"></a><span data-ttu-id="6f46b-149">Transférer un message électronique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="6f46b-149">Forward an email message by using EWS</span></span>
<span data-ttu-id="6f46b-150"><a name="bk_forwardews"> </a></span><span class="sxs-lookup"><span data-stu-id="6f46b-150"></span></span>

<span data-ttu-id="6f46b-151">L’exemple de code suivant montre comment transférer un message à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="6f46b-151">The following code example shows how to forward a message by using EWS.</span></span> <span data-ttu-id="6f46b-152">Utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) avec l’attribut **MessageDisposition** **SendAndSaveCopy** pour envoyer le message et enregistrez la réponse dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="6f46b-152">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="6f46b-153">L’élément [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) indique que l’élément est un message transféré.</span><span class="sxs-lookup"><span data-stu-id="6f46b-153">The [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) element indicates that the item is a forwarded message.</span></span> 
  
<span data-ttu-id="6f46b-154">C’est également la demande XML qui envoie de l’API managée EWS lors de l’appel du [Transférer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) ou la méthode [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6f46b-154">This is also the XML request that the EWS Managed API sends when calling either the [Forward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) or the [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) method.</span></span> 
  
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
      <m:Items>
        <t:ForwardItem>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:ReferenceItemId Id="AAAMkADE="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the forwarded email.</t:NewBodyContent>
        </t:ForwardItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f46b-155">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le message transféré a été créé et envoyé avec succès.</span><span class="sxs-lookup"><span data-stu-id="6f46b-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the forwarded message was created and sent successfully.</span></span>
  
<span data-ttu-id="6f46b-156">Si vous souhaitez ajouter une pièce jointe à votre message de réponse, appelez l’opération **CreateItem** , mais remplacez le **MessageDisposition** **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="6f46b-156">If you need to add an attachment to your response message, call the **CreateItem** operation, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="6f46b-157">Appelez ensuite l’opération [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , suivie de l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6f46b-157">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="find-the-message-last-replied-to-or-forwarded-by-using-the-ews-managed-api"></a><span data-ttu-id="6f46b-158">Rechercher le message dernière une réponse ou transférés à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6f46b-158">Find the message last replied to or forwarded by using the EWS Managed API</span></span>
<span data-ttu-id="6f46b-159"><a name="bk_findlast"> </a></span><span class="sxs-lookup"><span data-stu-id="6f46b-159"></span></span>

<span data-ttu-id="6f46b-160">L’exemple de code suivant montre comment rechercher le dernier verbe exécuté et l’heure du dernier verbe a été exécuté sur l’élément spécifié.</span><span class="sxs-lookup"><span data-stu-id="6f46b-160">The following code example shows how to find the last verb executed and the time the last verb was executed on the item specified.</span></span> <span data-ttu-id="6f46b-161">Cette méthode est appelée à partir d’autres exemples de code d’API managées dans cette rubrique pour vérifier que les éléments une réponse ou transférés ont été marqués comme une réponse ou transférés dans votre boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="6f46b-161">This method is called from other EWS Managed API code examples in this topic to verify that the items you replied to or forwarded were marked as replied to or forwarded in your Inbox.</span></span> 
  
<span data-ttu-id="6f46b-162">L’exemple utilise la propriété [PidTagLastVerbExecuted](http://msdn.microsoft.com/en-us/library/cc841968.aspx) (0x10820003) étendu pour déterminer si le message a été une réponse, un répondre à tous ou transfert et la [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x10820040) étendu de propriété pour déterminer le moment où le réponse ou le transfert a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6f46b-162">The example uses the [PidTagLastVerbExecuted](http://msdn.microsoft.com/en-us/library/cc841968.aspx) (0x10820003) extended property to determine whether the message was a reply, a reply all, or a forward, and the [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x10820040) extended property to determine when the reply or forward was sent.</span></span> 
  
```cs
public static void FindRecentlySent(EmailMessage messageToCheck)
{
    // Create extended property definitions for PidTagLastVerbExecuted and PidTagLastVerbExecutionTime.
    ExtendedPropertyDefinition PidTagLastVerbExecuted = new ExtendedPropertyDefinition(0x1081, MapiPropertyType.Integer);
    ExtendedPropertyDefinition PidTagLastVerbExecutionTime = new ExtendedPropertyDefinition(0x1082, MapiPropertyType.SystemTime);
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, PidTagLastVerbExecutionTime, PidTagLastVerbExecuted);
    messageToCheck = EmailMessage.Bind(service, messageToCheck.Id, propSet);
    // Determine the last verb executed on the message and display output.
    object responseType;
    if (messageToCheck.TryGetProperty(PidTagLastVerbExecuted, out responseType))
    {
        object ReplyTime = null;
        switch (((Int32)responseType))
        {
            case 102: Console.WriteLine("A reply was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 103: Console.WriteLine("A reply all was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 104: Console.WriteLine("The '" + messageToCheck.Subject.ToString() + "' email message was forwarded at");
                break;
        }
        if (messageToCheck.TryGetProperty(PidTagLastVerbExecutionTime, out ReplyTime))
        {
            Console.WriteLine(((DateTime)ReplyTime).ToString() + ".");
        }
    }
    else
    {
        Console.WriteLine("No changes were made to  '" + messageToCheck.Subject.ToString() + "'.");
    }
}
```

## <a name="see-also"></a><span data-ttu-id="6f46b-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6f46b-163">See also</span></span>


- [<span data-ttu-id="6f46b-164">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="6f46b-164">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="6f46b-165">Envoyer des messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6f46b-165">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
