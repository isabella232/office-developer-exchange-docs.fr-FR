---
title: Opération de GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Trouvez des informations sur l’opération EWS GetStreamingEvents.
ms.openlocfilehash: 27744ec40d7c7cb551f35ed5f6fcb726f23d4865
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530168"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="a91ba-103">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="a91ba-104">Trouvez des informations sur l’opération EWS **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="a91ba-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="a91ba-105">L’opération **GetStreamingEvents** est utilisée par les clients d’abonnements de diffusion en continu pour demander des notifications à partir du serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="a91ba-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="a91ba-106">La réponse **GetStreamingEvents** renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="a91ba-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="a91ba-107">Exemple de requête GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="a91ba-108">Description</span><span class="sxs-lookup"><span data-stu-id="a91ba-108">Description</span></span>

<span data-ttu-id="a91ba-109">L’exemple suivant d’une opération **GetStreamingEvents** indique comment demander les événements et les éléments qui sont associés à un abonnement identifié par l’identificateur d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a91ba-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a91ba-110">Code</span><span class="sxs-lookup"><span data-stu-id="a91ba-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="a91ba-111">Éléments de requête GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="a91ba-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="a91ba-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a91ba-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="a91ba-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="a91ba-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="a91ba-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="a91ba-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="a91ba-116">Exemple de réponse GetStreamingEvents réussi</span><span class="sxs-lookup"><span data-stu-id="a91ba-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="a91ba-117">Description</span><span class="sxs-lookup"><span data-stu-id="a91ba-117">Description</span></span>

<span data-ttu-id="a91ba-118">L’exemple suivant de réponse **GetStreamingEvents** indique les notifications envoyées au client lors de la réception d’un nouveau message électronique.</span><span class="sxs-lookup"><span data-stu-id="a91ba-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="a91ba-119">Elle inclut des notifications pour les événements suivants : CreatedEvent, NewMail et ModifiedEvent.</span><span class="sxs-lookup"><span data-stu-id="a91ba-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a91ba-120">Code</span><span class="sxs-lookup"><span data-stu-id="a91ba-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="a91ba-121">Éléments Response GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="a91ba-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="a91ba-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a91ba-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="a91ba-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="a91ba-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a91ba-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a91ba-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a91ba-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="a91ba-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="a91ba-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="a91ba-127">Notification</span><span class="sxs-lookup"><span data-stu-id="a91ba-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a91ba-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="a91ba-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="a91ba-129">Pour trouver d’autres options pour le message de réponse de l’opération **GetStreamingEvents** , explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="a91ba-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a91ba-130">Commencez par l’élément [notification](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="a91ba-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="a91ba-131">Exemple de réponse d’erreur GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a91ba-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="a91ba-132">Description</span><span class="sxs-lookup"><span data-stu-id="a91ba-132">Description</span></span>

<span data-ttu-id="a91ba-133">L’exemple suivant montre une réponse d’erreur à une requête **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="a91ba-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a91ba-134">Code</span><span class="sxs-lookup"><span data-stu-id="a91ba-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetStreamingEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="a91ba-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="a91ba-135">Remarks</span></span>

<span data-ttu-id="a91ba-136">Lors du traitement d’une demande **GetStreamingEvents** , le serveur d’accès au client effectue les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a91ba-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="a91ba-137">Le [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) de la demande est confirmé comme étant un abonnement valide hébergé sur le serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="a91ba-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="a91ba-138">Si ce n’est pas le cas, l’appel **GetStreamingEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="a91ba-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="a91ba-139">L’adresse SMTP de l’utilisateur authentifié pour la demande est validée pour disposer des droits d’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="a91ba-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="a91ba-140">Si ce n’est pas le cas, la demande **GetStreamingEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="a91ba-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="a91ba-141">La file d’attente d’abonnement est interrogée pour les événements qui attendent d’être envoyés au client.</span><span class="sxs-lookup"><span data-stu-id="a91ba-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="a91ba-142">Si la file d’attente n’est pas vide, les premiers événements 50 de la file d’attente sont extraits de la file d’attente et codés dans une notification.</span><span class="sxs-lookup"><span data-stu-id="a91ba-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="a91ba-143">Si aucun événement n’est trouvé dans la file d’attente, une [StatusEvent](statusevent.md) est générée et codée dans une réponse de notification.</span><span class="sxs-lookup"><span data-stu-id="a91ba-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="a91ba-144">La réponse de notification est renvoyée au client.</span><span class="sxs-lookup"><span data-stu-id="a91ba-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="a91ba-145">Les événements inclus dans la notification sont supprimés de la file d’attente d’abonnement et le dernier filigrane local du serveur d’accès au client pour l’abonnement est défini sur le filigrane du dernier événement renvoyé.</span><span class="sxs-lookup"><span data-stu-id="a91ba-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="a91ba-146">Le délai d’expiration de l’abonnement est réinitialisé.</span><span class="sxs-lookup"><span data-stu-id="a91ba-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="a91ba-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a91ba-147">See also</span></span>



[<span data-ttu-id="a91ba-148">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a91ba-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a91ba-149">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a91ba-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)

