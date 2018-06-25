---
title: Notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe9bde1e-da0e-413c-a109-077f399f67a3
description: Découvrez comment utiliser les API managées EWS pour s’abonner aux notifications de diffusion en continu et obtenir les événements.
ms.openlocfilehash: aad7604511687d1482914183979e954f79572af9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754938"
---
# <a name="stream-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange

Découvrez comment utiliser les API managées EWS pour s’abonner aux notifications de diffusion en continu et obtenir les événements.
  
EWS dans Exchange utilise transmettre en continu des notifications pour recevoir les notifications sont envoyées par le serveur via une connexion reste ouvert pour une période spécifiée.
  
Si vous êtes abonné à transmettre en continu des notifications à l’aide de l’API managées, vous [abonner et obtenir transmettre en continu des notifications](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamewsma) à l’aide de la méthode [SubscribeToStreamingNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) . Ensuite, vous créez une connexion à l’abonnement à l’aide de l’objet [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) . 
  
Pour vous abonner aux notifications de diffusion en continu à l’aide de EWS, vous [créez un abonnement](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamews) à l’aide de l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), d’analyser la réponse, puis [obtenir les notifications de diffusion en continu](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) à l’aide de l' [opération GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) demande. 
  
Une fois que le client reçoit des notifications d’éléments modifiés ou créés sur le serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser les modifications. 
  
## <a name="subscribe-to-and-get-streaming-notifications-by-using-the-ews-managed-api"></a>S’abonner à et obtenir la diffusion en continu des notifications à l’aide de l’API managée EWS
<a name="bk_cestreamewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [SubscribeToStreamingNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) s’abonner à des notifications pour tous les événements dans le dossier boîte de réception de diffusion en continu. Il crée ensuite une connexion pour l’abonnement en créant un objet [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) . Dans cet exemple, nous partons du principe que **service** est une liaison [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide. 
  
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

Une fois que vous avez reçu d’événements à partir du serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser les modifications avec le serveur. Utilisez une des méthodes de désabonnement répertoriés dans le [tableau 4](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire. 
  
## <a name="subscribe-to-streaming-notifications-by-using-ews"></a>S’abonner au flux de notifications à l’aide de EWS
<a name="bk_cestreamews"> </a>

L’exemple suivant montre une requête XML qui est envoyée par le client sur le serveur lorsque le client appelle l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) à s’abonner à tous les [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier boîte de réception. C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode [SubscribeToStreamingNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) pour vous abonner aux notifications de diffusion en continu. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

L’exemple XML suivant montre le message est envoyé à partir du serveur au client en réponse à la demande [Subscribe opération](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . L’inclusion de la valeur NoError pour l’élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès. L’élément [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie l’abonnement de notification de diffusion en continu sur le serveur. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Après avoir créé l’abonnement, vous pouvez désormais [obtenir les événements en flux continu](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) à l’aide du [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) renvoyé dans le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . 
  
## <a name="get-streaming-events-by-using-ews"></a>Obtenir de diffusion en continu des événements à l’aide de EWS
<a name="bk_cegetnotifsews"> </a>

L’exemple XML suivant montre le message de demande [d’opération GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) le client envoie au serveur pour obtenir des notifications pour le [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) renvoyé dans le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . La requête [d’opération GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) indique que la longueur de la connexion est long de 30 minutes. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

L’exemple XML suivant montre le message est envoyé à partir du serveur au client en réponse à la requête [d’opération GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) [GetStreamingEventsResponse](http://msdn.microsoft.com/library/ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2%28Office.15%29.aspx) . Il contient un CreatedEvent et un NewMailEvent pour l’élément et un ModifiedEvent pour le dossier qui se produisent lorsqu’un nouveau message est reçu. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Une fois que vous avez reçu d’événements à partir du serveur, l' [étape suivante](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) consiste à synchroniser les modifications avec le serveur. Utilisez l' [opération Annuler l’abonnement](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) à la fin de l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire. 
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_nextsteps"> </a>

Une fois que vous avez reçu, vous pouvez [synchroniser la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [synchroniser le contenu du dossier qui a été modifiée](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Extraction des notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

