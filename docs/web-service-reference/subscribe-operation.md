---
title: Opération d’abonnement
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: L’opération s’abonner permet de s’abonner à des notifications push ou extrait des applications clientes. Il est important de savoir que la structure des messages de demande et des réponses est différente selon le type de notification d’événement.
ms.openlocfilehash: f6cacab80c8ca2e505ab63a162a161fcf5de8585
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829619"
---
# <a name="subscribe-operation"></a><span data-ttu-id="38b64-104">Opération d’abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-104">Subscribe operation</span></span>

<span data-ttu-id="38b64-105">L’opération s’abonner permet de s’abonner à des notifications push ou extrait des applications clientes.</span><span class="sxs-lookup"><span data-stu-id="38b64-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="38b64-106">Il est important de savoir que la structure des messages de demande et des réponses est différente selon le type de notification d’événement.</span><span class="sxs-lookup"><span data-stu-id="38b64-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="38b64-107">Exemple de requête s’abonner abonnement extrait</span><span class="sxs-lookup"><span data-stu-id="38b64-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="38b64-108">Description</span><span class="sxs-lookup"><span data-stu-id="38b64-108">Description</span></span>

<span data-ttu-id="38b64-109">L’exemple de code suivant montre comment s’abonner à un abonnement notification d’événement.</span><span class="sxs-lookup"><span data-stu-id="38b64-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="38b64-110">L’abonnement informe l’application cliente si nouveau message est ajouté à la boîte de réception et si un élément est supprimé de la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="38b64-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="38b64-111">L’abonnement expire si le client ne demande pas d’informations sur les événements dans les dix minutes.</span><span class="sxs-lookup"><span data-stu-id="38b64-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="38b64-112">Si l’abonnement arrive à expiration, un nouvel abonnement doit être établi pour continuer à demander des notifications.</span><span class="sxs-lookup"><span data-stu-id="38b64-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="38b64-113">Code</span><span class="sxs-lookup"><span data-stu-id="38b64-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="38b64-114">Abonnement s’abonner à des éléments de demande</span><span class="sxs-lookup"><span data-stu-id="38b64-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="38b64-115">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="38b64-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="38b64-116">S’abonner</span><span class="sxs-lookup"><span data-stu-id="38b64-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="38b64-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="38b64-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="38b64-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="38b64-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="38b64-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="38b64-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="38b64-120">EventTypes</span><span class="sxs-lookup"><span data-stu-id="38b64-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="38b64-121">EventType</span><span class="sxs-lookup"><span data-stu-id="38b64-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="38b64-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="38b64-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="38b64-123">Pour trouver d’autres options pour le message de demande de l’opération de s’abonner, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="38b64-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="38b64-124">Démarrez au niveau de l’élément [PullSubscriptionRequest](pullsubscriptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="38b64-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="38b64-125">Exemple de réponse d’extraction abonnement associé réussie</span><span class="sxs-lookup"><span data-stu-id="38b64-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="38b64-126">Description</span><span class="sxs-lookup"><span data-stu-id="38b64-126">Description</span></span>

<span data-ttu-id="38b64-127">L’exemple suivant montre une réponse d’abonnement extrait réussie.</span><span class="sxs-lookup"><span data-stu-id="38b64-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="38b64-128">La réponse contient l’identificateur d’abonnement et filigrane qui est utilisée pour obtenir le tableau des événements qui sont associés à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="38b64-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="38b64-129">L’identificateur d’abonnement est également utilisé pour annuler l’abonnement d’un client à partir d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="38b64-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="38b64-130">Code</span><span class="sxs-lookup"><span data-stu-id="38b64-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="38b64-131">Extraire des éléments de réponse abonnement associé</span><span class="sxs-lookup"><span data-stu-id="38b64-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="38b64-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="38b64-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="38b64-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="38b64-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="38b64-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="38b64-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="38b64-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38b64-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38b64-136">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38b64-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="38b64-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38b64-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38b64-138">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="38b64-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="38b64-139">Filigrane</span><span class="sxs-lookup"><span data-stu-id="38b64-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="38b64-140">Exemple de réponse d’erreur d’abonnement s’abonner extraction</span><span class="sxs-lookup"><span data-stu-id="38b64-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="38b64-141">Description</span><span class="sxs-lookup"><span data-stu-id="38b64-141">Description</span></span>

<span data-ttu-id="38b64-142">L’exemple suivant montre une réponse d’erreur à la demande Subscribe.</span><span class="sxs-lookup"><span data-stu-id="38b64-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="38b64-143">L’erreur est provoquée par une tentative de s’abonner à des notifications à l’aide de l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="38b64-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="38b64-144">Code</span><span class="sxs-lookup"><span data-stu-id="38b64-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="38b64-145">Extraire des éléments de réponse d’erreur d’abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="38b64-146">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="38b64-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="38b64-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="38b64-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="38b64-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="38b64-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="38b64-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38b64-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38b64-150">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38b64-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="38b64-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="38b64-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="38b64-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38b64-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38b64-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="38b64-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="38b64-154">Exemple de requête push abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="38b64-155">Description</span><span class="sxs-lookup"><span data-stu-id="38b64-155">Description</span></span>

<span data-ttu-id="38b64-156">L’exemple de code suivant montre comment s’abonner à un abonnement de notification d’événement envoyé.</span><span class="sxs-lookup"><span data-stu-id="38b64-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="38b64-157">La demande identifie les dossiers à surveiller, les types d’événements à surveiller, la fréquence des notifications d’état et l’URL du service Web qui est à l’écoute des notifications push client.</span><span class="sxs-lookup"><span data-stu-id="38b64-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="38b64-158">Code</span><span class="sxs-lookup"><span data-stu-id="38b64-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="http://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="http://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="38b64-159">Commentaires</span><span class="sxs-lookup"><span data-stu-id="38b64-159">Comments</span></span>

<span data-ttu-id="38b64-160">Le client Web service doit être défini avant la notification push abonner demande est envoyé ; dans le cas contraire, la première notification ne sera pas être envoyée à un point de terminaison valide et les notifications push échoue.</span><span class="sxs-lookup"><span data-stu-id="38b64-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="38b64-161">Pour plus d’informations, voir [Application des exemples de Notification Push](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="38b64-161">For more information, see [Push Notification Sample Application](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="38b64-162">Un nouveau [SubscriptionId (GetEvents)](subscriptionid-getevents.md) est créé lorsque vous réabonner.</span><span class="sxs-lookup"><span data-stu-id="38b64-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="38b64-163">Utilisez la limite d’un abonnement précédente pour réabonner au niveau du point où l’abonnement précédente s’est terminée.</span><span class="sxs-lookup"><span data-stu-id="38b64-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="38b64-164">Ajouter des éléments de demande d’abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="38b64-165">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="38b64-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="38b64-166">S’abonner</span><span class="sxs-lookup"><span data-stu-id="38b64-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="38b64-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="38b64-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="38b64-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="38b64-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="38b64-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="38b64-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="38b64-170">EventTypes</span><span class="sxs-lookup"><span data-stu-id="38b64-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="38b64-171">EventType</span><span class="sxs-lookup"><span data-stu-id="38b64-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="38b64-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="38b64-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="38b64-173">URL</span><span class="sxs-lookup"><span data-stu-id="38b64-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="38b64-174">Exemple de réponse réussie d’un abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="38b64-175">Description</span><span class="sxs-lookup"><span data-stu-id="38b64-175">Description</span></span>

<span data-ttu-id="38b64-176">L’exemple suivant montre une réponse d’abonnement push ayant réussi.</span><span class="sxs-lookup"><span data-stu-id="38b64-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38b64-177">Code</span><span class="sxs-lookup"><span data-stu-id="38b64-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a><span data-ttu-id="38b64-178">Ajouter des éléments de réponse d’abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-178">Push Subscription response elements</span></span>

<span data-ttu-id="38b64-179">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="38b64-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="38b64-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="38b64-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="38b64-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="38b64-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="38b64-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38b64-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38b64-183">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38b64-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="38b64-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38b64-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38b64-185">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="38b64-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="38b64-186">Filigrane</span><span class="sxs-lookup"><span data-stu-id="38b64-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="38b64-187">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38b64-187">See also</span></span>



[<span data-ttu-id="38b64-188">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="38b64-189">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="38b64-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="38b64-190">À l’aide d’abonnement</span><span class="sxs-lookup"><span data-stu-id="38b64-190">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="38b64-191">Exemple d'application de notification Push</span><span class="sxs-lookup"><span data-stu-id="38b64-191">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

