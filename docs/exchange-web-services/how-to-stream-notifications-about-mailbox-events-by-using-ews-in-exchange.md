---
title: Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: fe9bde1e-da0e-413c-a109-077f399f67a3
description: Découvrez comment utiliser l’API managée EWS ou EWS pour vous abonner aux notifications de diffusion en continu et obtenir des événements.
localization_priority: Priority
ms.openlocfilehash: 97784be8ab13509f950355f532f97167e9b6f43e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527718"
---
# <a name="stream-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="90fa8-103">Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-103">Stream notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="90fa8-104">Découvrez comment utiliser l’API managée EWS ou EWS pour vous abonner aux notifications de diffusion en continu et obtenir des événements.</span><span class="sxs-lookup"><span data-stu-id="90fa8-104">Find out how to use the EWS Managed API or EWS to subscribe to streaming notifications and get events.</span></span>
  
<span data-ttu-id="90fa8-105">EWS dans Exchange utilise des notifications de diffusion en continu pour recevoir des notifications envoyées par le serveur via une connexion qui reste ouverte pendant une période de temps spécifiée.</span><span class="sxs-lookup"><span data-stu-id="90fa8-105">EWS in Exchange uses streaming notifications to receive notifications that are sent by the server through a connection that remains open for a specified period of time.</span></span>
  
<span data-ttu-id="90fa8-106">Si vous vous abonnez à des notifications de diffusion en continu à l’aide de l’API managée EWS, vous vous [Abonnez et obtenez des notifications de diffusion en continu](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamewsma) à l’aide de la méthode [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-106">If you're subscribing to streaming notifications by using the EWS Managed API, you [subscribe and get streaming notifications](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamewsma) by using the [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="90fa8-107">Vous créez ensuite une connexion à l’abonnement à l’aide de l’objet [méthode streamingsubscriptionconnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-107">You then create a connection to the subscription by using the [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="90fa8-108">Pour vous abonner aux notifications de diffusion en continu à l’aide d’EWS, vous [créez un abonnement](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamews) à l’aide de l' [opération subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), analysez la réponse, puis [obtenez les notifications de diffusion en continu](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) à l’aide de la demande d' [opération GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-108">To subscribe to streaming notifications by using EWS, you [create a subscription](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamews) by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the streaming notifications](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) by using the [GetStreamingEvents operation](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request.</span></span> 
  
<span data-ttu-id="90fa8-109">Une fois que le client reçoit des notifications d’éléments modifiées ou créées sur le serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser les modifications.</span><span class="sxs-lookup"><span data-stu-id="90fa8-109">After the client receives notifications of items changed or created on the server, the [next step](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) is to synchronize the changes.</span></span> 
  
## <a name="subscribe-to-and-get-streaming-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="90fa8-110">S’abonner à et obtenir des notifications de diffusion en continu à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="90fa8-110">Subscribe to and get streaming notifications by using the EWS Managed API</span></span>
<span data-ttu-id="90fa8-111"><a name="bk_cestreamewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="90fa8-111"><a name="bk_cestreamewsma"> </a></span></span>

<span data-ttu-id="90fa8-112">L’exemple de code suivant montre comment utiliser la méthode [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) pour s’abonner à des notifications de diffusion en continu pour tous les événements dans le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="90fa8-112">The following code example shows how to use the [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) method to subscribe to streaming notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="90fa8-113">Il crée ensuite une connexion pour l’abonnement en créant un objet [méthode streamingsubscriptionconnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-113">It then creates a connection for the subscription by creating a [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="90fa8-114">Dans cet exemple, nous partons du principe que le **service** est une liaison [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide.</span><span class="sxs-lookup"><span data-stu-id="90fa8-114">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to streaming notifications in the Inbox. 
StreamingSubscription = service.SubscribeToStreamingNotifications(
    new FolderId[] { WellKnownFolderName.Inbox },
    EventType.NewMail,
    EventType.Created,
    EventType.Deleted,
    EventType.Modified,
    EventType.Moved,
    EventType.Copied,
    EventType.FreeBusyChanged);
// Create a streaming connection to the service object, over which events are returned to the client.
// Keep the streaming connection open for 30 minutes.
StreamingSubscriptionConnection connection = new StreamingSubscriptionConnection(service, 30);
connection.AddSubscription(StreamingSubscription);
connection.OnNotificationEvent += OnNotificationEvent;
connection.OnDisconnect += OnDisconnect;
connection.Open();
```

<span data-ttu-id="90fa8-115">Une fois que vous avez reçu des événements du serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser ces modifications avec le serveur.</span><span class="sxs-lookup"><span data-stu-id="90fa8-115">After you have received events from the server, the [next step](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) is to synchronize those changes with the server.</span></span> <span data-ttu-id="90fa8-116">Utilisez l’une des méthodes unsubscribe indiquées dans le [tableau 4](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="90fa8-116">Use one of the unsubscribe methods listed in [Table 4](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-streaming-notifications-by-using-ews"></a><span data-ttu-id="90fa8-117">S’abonner à des notifications de diffusion en continu à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="90fa8-117">Subscribe to streaming notifications by using EWS</span></span>
<span data-ttu-id="90fa8-118"><a name="bk_cestreamews"> </a></span><span class="sxs-lookup"><span data-stu-id="90fa8-118"><a name="bk_cestreamews"> </a></span></span>

<span data-ttu-id="90fa8-119">L’exemple suivant montre une requête XML envoyée par le client au serveur lorsque le client appelle l' [opération subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) pour s’abonner à tous les [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="90fa8-119">The following example shows an XML request that is sent by the client to the server when the client calls the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) to subscribe to all [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder.</span></span> <span data-ttu-id="90fa8-120">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) pour vous abonner aux notifications de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="90fa8-120">This is also the XML request that the EWS Managed API sends when you use the [SubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) method to subscribe to streaming notifications.</span></span> 
  
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
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>CreatedEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
          <t:EventType>ModifiedEvent</t:EventType>
          <t:EventType>MovedEvent</t:EventType>
          <t:EventType>CopiedEvent</t:EventType>
          <t:EventType>FreeBusyChangedEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="90fa8-121">L’exemple de code XML suivant montre le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d' [opération subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-121">The following XML example shows the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) request.</span></span> <span data-ttu-id="90fa8-122">L’inclusion de la valeur NOERROR pour l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="90fa8-122">The inclusion of the NoError value for the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="90fa8-123">L’élément [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie de manière unique l’abonnement aux notifications de diffusion en continu sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="90fa8-123">The [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the streaming notification subscription on the server.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
          <m:SubscribeResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</m:SubscriptionId>
          </m:SubscribeResponseMessage>
        </m:ResponseMessages>
      </m:SubscribeResponse>
    </s:Body>
  </s:Envelope>
```

<span data-ttu-id="90fa8-124">Après avoir créé l’abonnement, vous pouvez [obtenir les événements transmis en continu](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) à l’aide de la [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) renvoyée dans le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-124">After creating the subscription, you can now [get the streamed events](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) by using the [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) returned in the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> 
  
## <a name="get-streaming-events-by-using-ews"></a><span data-ttu-id="90fa8-125">Obtenir des événements de diffusion en continu à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="90fa8-125">Get streaming events by using EWS</span></span>
<span data-ttu-id="90fa8-126"><a name="bk_cegetnotifsews"> </a></span><span class="sxs-lookup"><span data-stu-id="90fa8-126"><a name="bk_cegetnotifsews"> </a></span></span>

<span data-ttu-id="90fa8-127">L’exemple de code XML suivant montre le message de demande d' [opération GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) que le client envoie au serveur pour obtenir des notifications pour le [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) renvoyé dans le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-127">The following XML example shows the [GetStreamingEvents operation](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request message that the client sends to the server to get notifications for the [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) returned in the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="90fa8-128">La demande d' [opération GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) indique que la longueur de la connexion est de 30 minutes.</span><span class="sxs-lookup"><span data-stu-id="90fa8-128">The [GetStreamingEvents operation](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request indicates that the length of the connection is 30 minutes long.</span></span> 
  
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
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>30</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="90fa8-129">L’exemple de code XML suivant montre le message [GetStreamingEventsResponse](https://msdn.microsoft.com/library/ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d' [opération GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="90fa8-129">The following XML example shows the [GetStreamingEventsResponse](https://msdn.microsoft.com/library/ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2%28Office.15%29.aspx) message that is sent from the server to the client in response to the [GetStreamingEvents operation](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request.</span></span> <span data-ttu-id="90fa8-130">Elle contient un CreatedEvent et un NewMailEvent pour l’élément, ainsi qu’un ModifiedEvent pour le dossier, qui se produisent tous lors de la réception d’un nouveau message.</span><span class="sxs-lookup"><span data-stu-id="90fa8-130">It contains a CreatedEvent and a NewMailEvent for the item, and a ModifiedEvent for the folder, all of which occur when a new message is received.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <soap:Body xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</t:SubscriptionId>
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

Une fois que vous avez reçu des événements du serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser ces modifications avec le serveur. <span data-ttu-id="90fa8-132">Utilisez l' [opération de désinscription](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire.</span><span class="sxs-lookup"><span data-stu-id="90fa8-132">Use the [Unsubscribe operation](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="90fa8-133">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="90fa8-133">Next steps</span></span>
<span data-ttu-id="90fa8-134"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="90fa8-134"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="90fa8-135">Une fois que vous avez reçu les notifications, vous pouvez [synchroniser la hiérarchie des dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [synchroniser le contenu du dossier qui a été modifié](how-to-synchronize-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="90fa8-135">After you've received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="90fa8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="90fa8-136">See also</span></span>


- [<span data-ttu-id="90fa8-137">Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-137">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="90fa8-138">Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-138">Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="90fa8-139">Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-139">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="90fa8-140">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-140">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="90fa8-141">Synchronisation de la boîte aux lettres et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="90fa8-141">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

