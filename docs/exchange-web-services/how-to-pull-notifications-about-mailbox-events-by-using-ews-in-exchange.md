---
title: Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Découvrez comment utiliser l’API gérée EWS ou EWS pour vous abonner aux notifications de pull et obtenir des événements.
ms.openlocfilehash: eb694eddd16567e42ccc43b2854f0432c54dc6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513100"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange

Découvrez comment utiliser l’API gérée EWS ou EWS pour vous abonner aux notifications de pull et obtenir des événements.
  
EWS dans Exchange utilise des notifications de pull pour permettre aux clients de demander (ou de tirer) des notifications concernant les modifications apportées à la boîte aux lettres du serveur au client.
  
Si vous vous abonnez à des notifications de pull à l’aide de l’API gérée EWS, vous vous abonnez et recevez des [notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) de pull à l’aide de la méthode [SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) Vous obtenez ensuite des événements à partir du serveur à l’aide de [la méthode GetEvents.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) 
  
Pour vous abonner aux notifications de [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) pull à l’aide d’EWS, vous créez un abonnement à l’aide de l’opération s’abonner, [](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)parse la réponse, puis obtenez les [notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) à l’aide de l’opération [GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
Une fois que le client a reçu des notifications d’éléments modifiés ou créés sur le serveur, il peut [synchroniser les modifications.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>S’abonner et recevoir des notifications de pull à l’aide de l’API gérée EWS
<a name="bk_cepullewsma"> </a>

L’exemple de code suivant montre comment utiliser la [méthode SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) pour s’abonner aux notifications de pull pour tous les événements dans le dossier Boîte de réception. L’exemple utilise ensuite la [méthode GetEvents pour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) récupérer des événements à partir du serveur. Dans cet exemple, nous partons du principe **que le service** est une liaison [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide. 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

Après avoir reçu un événement du serveur, vous pouvez synchroniser ces modifications [avec le serveur.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) Utilisez l’une des méthodes de désabonnement spécifiées dans Comment puis-je me désabonner aux [notifications ?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>S’abonner aux notifications de pull à l’aide d’EWS
<a name="bk_cepullews"> </a>

L’exemple suivant montre la demande XML à envoyer au serveur pour s’abonner à tous les [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier Boîte de réception à l’aide de [l’opération Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Il s’agit également de la demande XML que l’API gérée EWS envoie lors de l’abonnement aux notifications de pull à l’aide de la méthode [SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) 
  
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

L’exemple XML suivant montre le message [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) qui est envoyé du serveur au client en réponse à la demande **d’opération Subscribe.** L’inclusion de la valeur NoError pour [l’élément ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès. [L’élément SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie de manière unique l’abonnement de notification de pull sur le serveur. [L’élément Filigrane](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) représente un signet dans la file d’attente des événements de boîte aux lettres. 
  
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

Après avoir créé l’abonnement, vous pouvez désormais obtenir des événements à l’aide de **l’SubscriptionId** renvoyé dans le message **SubscribeResponse.** 
  
## <a name="get-pull-notifications-by-using-ews"></a>Obtenir des notifications de pull à l’aide d’EWS
<a name="bk_getpull"> </a>

L’exemple XML suivant montre le message de demande d’opération [GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) qui est envoyé du client au serveur pour obtenir des notifications pour [l’SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) qui est renvoyé dans le message [SubscribeResponse.](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) Pour la première **demande GetEvents,** utilisez le [filigrane](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) renvoyé dans la réponse **d’abonnement.** Pour les **demandes GetEvents suivantes,** utilisez le dernier filigrane qui a été renvoyé dans la demande **GetEvents** précédente.  
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

L’exemple XML suivant montre le message de réponse **GetEvents** qui est envoyé du serveur au client. Chaque **réponse GetEvents** inclut des informations sur un ou plusieurs événements. Un **filigrane** est renvoyé pour chaque événement. Le dernier **filigrane** doit être enregistré et utilisé dans la demande **GetEvents** suivante. Si aucun événement de magasin ne s’est produit depuis la dernière **demande GetEvents,** un événement d’état est renvoyé. 
  
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

Une fois que vous avez reçu un événement du serveur, [synchronisez les modifications avec le client.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) Utilisez [l’opération De désabonnement](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) pour mettre fin à l’abonnement avec le serveur lorsque l’abonnement n’est plus nécessaire. 
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_nextsteps"> </a>

Une fois les notifications reçues, vous pouvez [synchroniser](how-to-synchronize-folders-by-using-ews-in-exchange.md) la hiérarchie de dossiers ou synchroniser le contenu du [dossier qui a été modifié.](how-to-synchronize-items-by-using-ews-in-exchange.md)
  
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

