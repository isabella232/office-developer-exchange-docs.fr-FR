---
title: Opération de GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: L’opération GetEvents est utilisée par les clients d’abonnements extraits pour demander des notifications à partir du serveur d’accès au client. La réponse de l’opération GetEvents renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification.
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462513"
---
# <a name="getevents-operation"></a><span data-ttu-id="4f356-104">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-104">GetEvents operation</span></span>

<span data-ttu-id="4f356-105">L’opération **GetEvents** est utilisée par les clients d’abonnements extraits pour demander des notifications à partir du serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="4f356-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="4f356-106">La réponse de l’opération **GetEvents** renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="4f356-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="4f356-107">L’opération **DeleteUserConfiguration** déclenchera un événement Move pour le système de notification d’événements.</span><span class="sxs-lookup"><span data-stu-id="4f356-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="4f356-108">L’objet de configuration utilisateur est déplacé vers la benne.</span><span class="sxs-lookup"><span data-stu-id="4f356-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4f356-109">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f356-109">Remarks</span></span>

<span data-ttu-id="4f356-110">Les modifications apportées aux éléments de calendrier peuvent entraîner la génération de plusieurs événements.</span><span class="sxs-lookup"><span data-stu-id="4f356-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="4f356-111">Ces événements sont le résultat des éléments temporaires créés dans la boîte aux lettres, des éléments de stockage des données de disponibilité modifiés dans le cadre des opérations de calendrier normales ou des deux.</span><span class="sxs-lookup"><span data-stu-id="4f356-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="4f356-112">Événements de la classe d’élément «IPM. SchedulePlus. FreeBusy. BinaryData "doit être ignoré par les clients de service Web.</span><span class="sxs-lookup"><span data-stu-id="4f356-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="4f356-113">Ces éléments temporaires sont supprimés après leur création ; par conséquent, si vous tentez de récupérer ces éléments, une erreur est renvoyée, indiquant que l’élément est introuvable.</span><span class="sxs-lookup"><span data-stu-id="4f356-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="4f356-114">Exemple de requête GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="4f356-115">Description</span><span class="sxs-lookup"><span data-stu-id="4f356-115">Description</span></span>

<span data-ttu-id="4f356-116">L’exemple suivant montre comment demander les événements et les éléments qui sont associés à un abonnement identifié par l’identificateur d’abonnement et le filigrane.</span><span class="sxs-lookup"><span data-stu-id="4f356-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f356-117">Code</span><span class="sxs-lookup"><span data-stu-id="4f356-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="4f356-118">Éléments de requête GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-118">GetEvents Request Elements</span></span>

<span data-ttu-id="4f356-119">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="4f356-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4f356-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="4f356-121">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="4f356-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="4f356-122">Watermark</span><span class="sxs-lookup"><span data-stu-id="4f356-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="4f356-123">Exemple de réponse GetEvents réussi</span><span class="sxs-lookup"><span data-stu-id="4f356-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="4f356-124">Description</span><span class="sxs-lookup"><span data-stu-id="4f356-124">Description</span></span>

<span data-ttu-id="4f356-125">L’exemple suivant d’une réponse affiche une notification de l’existence de deux nouveaux messages électroniques depuis que la dernière demande de notification a été envoyée au serveur.</span><span class="sxs-lookup"><span data-stu-id="4f356-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="4f356-126">Code</span><span class="sxs-lookup"><span data-stu-id="4f356-126">Code</span></span>

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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4f356-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="4f356-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="4f356-128">Les identificateurs d’éléments et de dossiers ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4f356-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="4f356-129">Éléments de réponse GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-129">GetEvents response elements</span></span>

<span data-ttu-id="4f356-130">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="4f356-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4f356-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4f356-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4f356-132">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="4f356-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="4f356-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4f356-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4f356-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4f356-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="4f356-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4f356-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4f356-136">Notification</span><span class="sxs-lookup"><span data-stu-id="4f356-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="4f356-137">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="4f356-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="4f356-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="4f356-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="4f356-139">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="4f356-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="4f356-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="4f356-141">Watermark</span><span class="sxs-lookup"><span data-stu-id="4f356-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="4f356-142">Dates</span><span class="sxs-lookup"><span data-stu-id="4f356-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="4f356-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="4f356-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="4f356-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="4f356-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="4f356-145">Pour rechercher d’autres options pour le message de réponse de l’opération **GetEvents** , explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="4f356-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="4f356-146">Commencez par l’élément [notification](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="4f356-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="4f356-147">Exemple de réponse d’erreur GetEvents</span><span class="sxs-lookup"><span data-stu-id="4f356-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="4f356-148">Description</span><span class="sxs-lookup"><span data-stu-id="4f356-148">Description</span></span>

<span data-ttu-id="4f356-149">L’exemple suivant montre une réponse d’erreur à une demande **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="4f356-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4f356-150">Code</span><span class="sxs-lookup"><span data-stu-id="4f356-150">Code</span></span>

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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="4f356-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f356-151">Remarks</span></span>

<span data-ttu-id="4f356-152">Lors du traitement d’une demande **GetEvents** , le serveur d’accès au client effectue les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="4f356-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="4f356-153">Le SubscriptionID de la demande est confirmé comme étant un abonnement valide qui est hébergé sur le serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="4f356-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="4f356-154">Si ce n’est pas le cas, l’appel **GetEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="4f356-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="4f356-155">L’adresse SMTP de l’utilisateur authentifié pour la demande est comparée à l’adresse SMTP de l’utilisateur qui a créé l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="4f356-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="4f356-156">Si elles ne correspondent pas, la demande **GetEvents** échoue.</span><span class="sxs-lookup"><span data-stu-id="4f356-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="4f356-157">La file d’attente d’abonnement est interrogée pour les événements qui attendent d’être envoyés au client.</span><span class="sxs-lookup"><span data-stu-id="4f356-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="4f356-158">Si la file d’attente n’est pas vide, les premiers événements 50 de la file d’attente sont extraits de la file d’attente et codés dans une notification.</span><span class="sxs-lookup"><span data-stu-id="4f356-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="4f356-159">Si aucun événement n’est trouvé dans la file d’attente, une StatusEvent est générée et codée dans une réponse de notification.</span><span class="sxs-lookup"><span data-stu-id="4f356-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="4f356-160">La réponse de notification est renvoyée au client.</span><span class="sxs-lookup"><span data-stu-id="4f356-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="4f356-161">Les événements inclus dans la notification sont supprimés de la file d’attente d’abonnement et le dernier filigrane local du serveur d’accès au client pour l’abonnement est défini sur le filigrane du dernier événement renvoyé.</span><span class="sxs-lookup"><span data-stu-id="4f356-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="4f356-162">Le délai d’expiration de l’abonnement est réinitialisé.</span><span class="sxs-lookup"><span data-stu-id="4f356-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="4f356-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f356-163">See also</span></span>



[<span data-ttu-id="4f356-164">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4f356-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="4f356-165">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4f356-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="4f356-166">Utilisation des abonnements extraits</span><span class="sxs-lookup"><span data-stu-id="4f356-166">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

