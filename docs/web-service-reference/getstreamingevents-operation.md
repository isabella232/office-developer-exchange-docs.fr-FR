---
title: Opération GetStreamingEvents
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
description: Opération de recherche plus d’informations sur la GetStreamingEvents EWS.
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827673"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="adbfd-103">Opération GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="adbfd-104">Trouvez des informations sur l’opération EWS **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="adbfd-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="adbfd-105">L’opération **GetStreamingEvents** est utilisée par la diffusion en continu des clients de l’abonnement pour demander des notifications à partir du serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="adbfd-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="adbfd-106">La réponse **GetStreamingEvents** renvoie un tableau d’éléments et les événements qui se sont produites dans une boîte aux lettres depuis le dernier la notification.</span><span class="sxs-lookup"><span data-stu-id="adbfd-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="adbfd-107">Exemple de requête GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="adbfd-108">Description</span><span class="sxs-lookup"><span data-stu-id="adbfd-108">Description</span></span>

<span data-ttu-id="adbfd-109">Une opération **GetStreamingEvents** l’exemple suivant montre comment demander les événements et les éléments qui sont associés à un abonnement identifié par l’identificateur d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="adbfd-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adbfd-110">Code</span><span class="sxs-lookup"><span data-stu-id="adbfd-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="adbfd-111">Éléments de requête GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="adbfd-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="adbfd-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="adbfd-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="adbfd-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="adbfd-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="adbfd-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="adbfd-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="adbfd-116">Exemple de réponse GetStreamingEvents réussie</span><span class="sxs-lookup"><span data-stu-id="adbfd-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="adbfd-117">Description</span><span class="sxs-lookup"><span data-stu-id="adbfd-117">Description</span></span>

<span data-ttu-id="adbfd-118">L’exemple suivant d’une réponse **GetStreamingEvents** montre les notifications sont envoyées au client lorsqu’un nouveau message électronique est reçu.</span><span class="sxs-lookup"><span data-stu-id="adbfd-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="adbfd-119">Il inclut des notifications pour les événements suivants : CreatedEvent, NewMail et ModifiedEvent.</span><span class="sxs-lookup"><span data-stu-id="adbfd-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adbfd-120">Code</span><span class="sxs-lookup"><span data-stu-id="adbfd-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="adbfd-121">Éléments de réponse GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="adbfd-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="adbfd-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="adbfd-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="adbfd-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="adbfd-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="adbfd-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="adbfd-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="adbfd-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="adbfd-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="adbfd-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="adbfd-127">Notification</span><span class="sxs-lookup"><span data-stu-id="adbfd-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="adbfd-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="adbfd-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="adbfd-129">Pour trouver d’autres options pour le message de réponse de l’opération **GetStreamingEvents** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="adbfd-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="adbfd-130">Démarrez au niveau de l’élément de [Notification](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="adbfd-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="adbfd-131">Exemple de réponse d’erreur GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="adbfd-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="adbfd-132">Description</span><span class="sxs-lookup"><span data-stu-id="adbfd-132">Description</span></span>

<span data-ttu-id="adbfd-133">L’exemple suivant montre une réponse d’erreur à une demande de **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="adbfd-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adbfd-134">Code</span><span class="sxs-lookup"><span data-stu-id="adbfd-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a><span data-ttu-id="adbfd-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="adbfd-135">Remarks</span></span>

<span data-ttu-id="adbfd-136">Lors du traitement d’une demande **GetStreamingEvents** , le serveur d’accès au Client effectue les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="adbfd-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="adbfd-137">Le [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) de la demande est confirmé comme étant un abonnement valide qui est hébergé sur le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="adbfd-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="adbfd-138">S’il n’est pas le cas, l’appel **GetStreamingEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="adbfd-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="adbfd-139">L’adresse SMTP de l’utilisateur authentifié pour la demande est validé pour les droits de l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="adbfd-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="adbfd-140">Si ce n’est pas le cas, la demande **GetStreamingEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="adbfd-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="adbfd-141">La file d’attente de l’abonnement est interrogé pour les événements qui sont en attente d’être envoyées au client.</span><span class="sxs-lookup"><span data-stu-id="adbfd-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="adbfd-142">Si la file d’attente n’est pas vide, les 50 premiers événements à partir de la file d’attente sont extraites de la file d’attente et codés dans une notification.</span><span class="sxs-lookup"><span data-stu-id="adbfd-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="adbfd-143">Si aucun événement n’est détectée dans la file d’attente, un [StatusEvent](statusevent.md) est généré et codé en réponse à une notification.</span><span class="sxs-lookup"><span data-stu-id="adbfd-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="adbfd-144">La réponse de notification est retournée au client.</span><span class="sxs-lookup"><span data-stu-id="adbfd-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="adbfd-145">Les événements qui sont inclus dans la notification sont supprimés de la file d’attente d’abonnement et la limite de serveur local dernier accès au Client pour l’abonnement est définie sur la limite du dernier événement qui est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="adbfd-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="adbfd-146">Le délai d’expiration de l’abonnement est réinitialisé.</span><span class="sxs-lookup"><span data-stu-id="adbfd-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="adbfd-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="adbfd-147">See also</span></span>



[<span data-ttu-id="adbfd-148">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="adbfd-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="adbfd-149">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="adbfd-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)

