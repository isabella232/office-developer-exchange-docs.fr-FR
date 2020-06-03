---
title: Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Découvrez comment utiliser l’API managée EWS ou EWS pour vous abonner aux notifications de type pull et obtenir des événements.
ms.openlocfilehash: 3d77c0d4efb8fc853eea64ff2429af5c3dbead27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456731"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="86aef-103">Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-103">Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="86aef-104">Découvrez comment utiliser l’API managée EWS ou EWS pour vous abonner aux notifications de type pull et obtenir des événements.</span><span class="sxs-lookup"><span data-stu-id="86aef-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="86aef-105">EWS dans Exchange utilise des notifications de type pull pour permettre aux clients de demander (ou d’extraire) des notifications sur les modifications apportées à la boîte aux lettres à partir du serveur vers le client.</span><span class="sxs-lookup"><span data-stu-id="86aef-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="86aef-106">Si vous vous abonnez à des notifications d’extraction à l’aide de l’API managée EWS, vous vous [Abonnez et recevez des notifications d’extraction](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) à l’aide de la méthode [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="86aef-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="86aef-107">Vous obtenez ensuite des événements à partir du serveur à l’aide de la méthode [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="86aef-107">You then get events from the server by using the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="86aef-108">Pour vous abonner aux notifications d’extraction à l’aide d’EWS, vous [créez un abonnement](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) à l’aide de l' [opération subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), analysez la réponse, puis [obtenez les notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) à l’aide de l' [opération GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="86aef-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="86aef-109">Une fois que le client reçoit des notifications d’éléments qui ont été modifiés ou créés sur le serveur, il peut ensuite [synchroniser les modifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="86aef-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="86aef-110">S’abonner à et obtenir des notifications d’extraction à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="86aef-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="86aef-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="86aef-111"><a name="bk_cepullewsma"> </a></span></span>

<span data-ttu-id="86aef-112">L’exemple de code suivant montre comment utiliser la méthode [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) pour s’abonner à des notifications de type pull pour tous les événements dans le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="86aef-112">The following code example shows how to use the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="86aef-113">L’exemple utilise ensuite la méthode [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) pour récupérer des événements à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="86aef-113">The example then uses the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="86aef-114">Dans cet exemple, nous partons du principe que le **service** est une liaison [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide.</span><span class="sxs-lookup"><span data-stu-id="86aef-114">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="86aef-115">Une fois que vous avez reçu un événement du serveur, vous pouvez [synchroniser ces modifications avec le serveur](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="86aef-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="86aef-116">Utilisez l’une des méthodes unsubscribe spécifiées dans [Comment annuler l’abonnement aux notifications ?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="86aef-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="86aef-117">S’abonner aux notifications d’extraction à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="86aef-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="86aef-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="86aef-118"><a name="bk_cepullews"> </a></span></span>

<span data-ttu-id="86aef-119">L’exemple suivant montre la requête XML à envoyer au serveur pour s’abonner à tous les [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier boîte de réception à l’aide de l' [opération subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="86aef-119">The following example shows the XML request to send to the server to subscribe to all [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span></span> <span data-ttu-id="86aef-120">Il s’agit également de la demande XML que l’API managée EWS envoie lorsqu’elle s’abonne à des notifications de type pull à l’aide de la méthode [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="86aef-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="https://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

<span data-ttu-id="86aef-121">L’exemple de code XML suivant montre le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d’opération **subscribe** .</span><span class="sxs-lookup"><span data-stu-id="86aef-121">The following XML example shows the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="86aef-122">L’inclusion de la valeur NOERROR pour l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="86aef-122">The inclusion of the NoError value for the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="86aef-123">L’élément [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie de manière unique l’abonnement aux notifications de type pull sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="86aef-123">The [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="86aef-124">L’élément de [filigrane](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) représente un signet dans la file d’attente d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="86aef-124">The [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

<span data-ttu-id="86aef-125">Après avoir créé l’abonnement, vous pouvez désormais obtenir des événements à l’aide de l' **SubscriptionId** renvoyé dans le message **SubscribeResponse** .</span><span class="sxs-lookup"><span data-stu-id="86aef-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="86aef-126">Obtenir des notifications d’extraction à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="86aef-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="86aef-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="86aef-127"><a name="bk_getpull"> </a></span></span>

<span data-ttu-id="86aef-128">L’exemple de code XML suivant montre le message d' [opération GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) envoyé par le client au serveur pour obtenir des notifications pour le [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) renvoyé dans le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="86aef-128">The following XML example shows the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="86aef-129">Pour la première demande **GetEvents** , utilisez le [filigrane](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) renvoyé dans la réponse **subscribe** .</span><span class="sxs-lookup"><span data-stu-id="86aef-129">For the first **GetEvents** request, use the [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="86aef-130">Pour les demandes **GetEvents** ultérieures, utilisez le dernier **filigrane** qui a été renvoyé dans la demande **GetEvents** précédente.</span><span class="sxs-lookup"><span data-stu-id="86aef-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="86aef-131">L’exemple de code XML suivant montre le message de réponse **GetEvents** envoyé par le serveur au client.</span><span class="sxs-lookup"><span data-stu-id="86aef-131">The following XML example shows the **GetEvents** response message that is sent from the server to the client.</span></span> <span data-ttu-id="86aef-132">Chaque réponse **GetEvents** inclut des informations sur un ou plusieurs événements.</span><span class="sxs-lookup"><span data-stu-id="86aef-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="86aef-133">Un **filigrane** est renvoyé pour chaque événement.</span><span class="sxs-lookup"><span data-stu-id="86aef-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="86aef-134">Le dernier **filigrane** doit être enregistré et utilisé dans la prochaine demande **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="86aef-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="86aef-135">Si aucun événement de magasin ne s’est produit depuis la dernière demande **GetEvents** , un événement d’État est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="86aef-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="https://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Watermark>AAAAAHMhAAAAAAAAAQ==</Watermark>
          <TimeStamp>2013-09-15T21:37:01Z</TimeStamp>
          <ItemId Id="AAAtA=" ChangeKey="CQAAAA==" />
          <ParentFolderId Id="AQAtAEFkbWA==" ChangeKey="AQAAAA==" />
        </NewMailEvent>
      </Notification>
    </GetEventsResponseMessage>
  </ResponseMessages>
</GetEventsResponse>
```

Une fois que vous avez reçu un événement du serveur, [synchronisez les modifications sur le client](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). <span data-ttu-id="86aef-137">Utilisez l' [opération de désinscription](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="86aef-137">Use the [Unsubscribe operation](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="86aef-138">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="86aef-138">Next steps</span></span>
<span data-ttu-id="86aef-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="86aef-139"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="86aef-140">Une fois que vous avez reçu les notifications, vous pouvez [synchroniser la hiérarchie des dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [synchroniser le contenu du dossier qui a été modifié](how-to-synchronize-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="86aef-140">After you're received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="86aef-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86aef-141">See also</span></span>


- [<span data-ttu-id="86aef-142">Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="86aef-143">Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-143">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="86aef-144">Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-144">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="86aef-145">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="86aef-146">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="86aef-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

