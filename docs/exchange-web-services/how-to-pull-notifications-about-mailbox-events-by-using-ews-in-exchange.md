---
title: Extraction des notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Découvrez comment utiliser les API managées EWS s’abonner à des notifications de type pull et obtenir les événements.
ms.openlocfilehash: 6a04aaf0102c149691a30c2bd2f499e03265bce8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754927"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="89473-103">Extraction des notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-103">Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="89473-104">Découvrez comment utiliser les API managées EWS s’abonner à des notifications de type pull et obtenir les événements.</span><span class="sxs-lookup"><span data-stu-id="89473-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="89473-105">EWS dans Exchange utilise des notifications de type pull pour permettre aux clients à la demande (ou extraction) des notifications sur les modifications apportées à la boîte aux lettres à partir du serveur au client.</span><span class="sxs-lookup"><span data-stu-id="89473-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="89473-106">Si vous vous abonnez aux notifications extrait à l’aide de l’API managées, vous [abonner à et obtenir des notifications de type pull](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) à l’aide de la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="89473-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="89473-107">Puis, vous obtenez les événements à partir du serveur à l’aide de la méthode [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="89473-107">You then get events from the server by using the [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="89473-108">Pour vous abonner à des notifications de type pull à l’aide de EWS, vous [créez un abonnement](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) à l’aide de l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), d’analyser la réponse, puis [obtenir les notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) à l’aide de l' [opération GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="89473-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="89473-109">Lorsque le client reçoit des notifications d’éléments qui sont modifiés ou créés sur le serveur, il peut ensuite [synchroniser les modifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="89473-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="89473-110">S’abonner à et obtenir des notifications de type pull à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="89473-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="89473-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="89473-111"></span></span>

<span data-ttu-id="89473-112">L’exemple de code suivant montre comment utiliser la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) pour vous abonner aux notifications d’extraction de tous les événements dans le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="89473-112">The following code example shows how to use the [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="89473-113">L’exemple utilise ensuite la méthode [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) à récupérer des événements à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="89473-113">The example then uses the [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="89473-114">Dans cet exemple, nous partons du principe que **service** est une liaison [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide.</span><span class="sxs-lookup"><span data-stu-id="89473-114">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="89473-115">Une fois que vous recevez un événement à partir du serveur, vous pouvez [synchroniser ces modifications avec le serveur](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="89473-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="89473-116">Utilisez une des méthodes d’abonnement spécifiés dans [comment pour désinscrire aux notifications ?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="89473-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="89473-117">S’abonner aux notifications de type pull à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="89473-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="89473-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="89473-118"></span></span>

<span data-ttu-id="89473-119">L’exemple suivant montre la demande XML à envoyer au serveur pour vous abonner à tous les [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier boîte de réception à l’aide de l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="89473-119">The following example shows the XML request to send to the server to subscribe to all [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span></span> <span data-ttu-id="89473-120">C’est également la demande XML qui envoie de l’API managée EWS lors de l’abonnement aux notifications de type pull à l’aide de la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="89473-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="http://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

<span data-ttu-id="89473-121">L’exemple XML suivant montre le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) qui est envoyé à partir du serveur au client en réponse à la requête d’opération **s’abonner** .</span><span class="sxs-lookup"><span data-stu-id="89473-121">The following XML example shows the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="89473-122">L’inclusion de la valeur NoError pour l’élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="89473-122">The inclusion of the NoError value for the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="89473-123">L’élément [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie l’abonnement de notification sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="89473-123">The [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="89473-124">L’élément [filigrane](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) représente un signet dans la file d’attente des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="89473-124">The [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

<span data-ttu-id="89473-125">Après avoir créé l’abonnement, vous pouvez désormais obtenir les événements à l’aide du **SubscriptionId** qui est renvoyé dans le message **SubscribeResponse** .</span><span class="sxs-lookup"><span data-stu-id="89473-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="89473-126">Obtenir des notifications de type pull à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="89473-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="89473-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="89473-127"></span></span>

<span data-ttu-id="89473-128">L’exemple XML suivant montre le message de demande [d’opération GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) est envoyé à partir du client sur le serveur pour obtenir des notifications pour le [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) qui est renvoyé dans le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="89473-128">The following XML example shows the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="89473-129">Pour la première demande **GetEvents** , utilisez le [filigrane](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retourné dans la réponse de **s’abonner** .</span><span class="sxs-lookup"><span data-stu-id="89473-129">For the first **GetEvents** request, use the [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="89473-130">Pour les demandes **GetEvents** suivantes, utilisez le dernier **filigrane** qui a été retournée dans la demande **GetEvents** précédente.</span><span class="sxs-lookup"><span data-stu-id="89473-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="89473-131">L’exemple XML suivant montre le message de réponse **GetEvents** qui est envoyé à partir du serveur au client.</span><span class="sxs-lookup"><span data-stu-id="89473-131">The following XML example shows the **GetEvents** response message that is sent from the server to the client.</span></span> <span data-ttu-id="89473-132">Chaque réponse **GetEvents** consacrée des informations sur un ou plusieurs événements.</span><span class="sxs-lookup"><span data-stu-id="89473-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="89473-133">Un **filigrane** est renvoyé pour chaque événement.</span><span class="sxs-lookup"><span data-stu-id="89473-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="89473-134">Le dernier **filigrane** doit être enregistré et utilisé dans la demande **GetEvents** suivante.</span><span class="sxs-lookup"><span data-stu-id="89473-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="89473-135">Si aucun événement magasin n’ont été effectuées depuis la dernière demande **GetEvents** , un événement d’état est retourné.</span><span class="sxs-lookup"><span data-stu-id="89473-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="http://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

Après avoir reçu un événement à partir du serveur, [synchroniser les modifications sur le client](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). <span data-ttu-id="89473-137">Utilisez l' [opération Annuler l’abonnement](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) à la fin de l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="89473-137">Use the [Unsubscribe operation](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="89473-138">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="89473-138">Next steps</span></span>
<span data-ttu-id="89473-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="89473-139"></span></span>

<span data-ttu-id="89473-140">Une fois que vous avez reçu les notifications, vous pouvez [synchroniser la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [synchroniser le contenu du dossier qui a été modifiée](how-to-synchronize-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="89473-140">After you're received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="89473-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89473-141">See also</span></span>


- [<span data-ttu-id="89473-142">Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="89473-143">Notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-143">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="89473-144">Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-144">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="89473-145">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="89473-146">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="89473-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

