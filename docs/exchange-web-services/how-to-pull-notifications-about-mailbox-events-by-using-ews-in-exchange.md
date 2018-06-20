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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754927"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Extraction des notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange

Découvrez comment utiliser les API managées EWS s’abonner à des notifications de type pull et obtenir les événements.
  
EWS dans Exchange utilise des notifications de type pull pour permettre aux clients à la demande (ou extraction) des notifications sur les modifications apportées à la boîte aux lettres à partir du serveur au client.
  
Si vous vous abonnez aux notifications extrait à l’aide de l’API managées, vous [abonner à et obtenir des notifications de type pull](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) à l’aide de la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . Puis, vous obtenez les événements à partir du serveur à l’aide de la méthode [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) . 
  
Pour vous abonner à des notifications de type pull à l’aide de EWS, vous [créez un abonnement](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) à l’aide de l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), d’analyser la réponse, puis [obtenir les notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) à l’aide de l' [opération GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
Lorsque le client reçoit des notifications d’éléments qui sont modifiés ou créés sur le serveur, il peut ensuite [synchroniser les modifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>S’abonner à et obtenir des notifications de type pull à l’aide de l’API managée EWS
<a name="bk_cepullewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) pour vous abonner aux notifications d’extraction de tous les événements dans le dossier boîte de réception. L’exemple utilise ensuite la méthode [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) à récupérer des événements à partir du serveur. Dans cet exemple, nous partons du principe que **service** est une liaison [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide. 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

Une fois que vous recevez un événement à partir du serveur, vous pouvez [synchroniser ces modifications avec le serveur](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Utilisez une des méthodes d’abonnement spécifiés dans [comment pour désinscrire aux notifications ?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) pour mettre fin à l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>S’abonner aux notifications de type pull à l’aide de EWS
<a name="bk_cepullews"> </a>

L’exemple suivant montre la demande XML à envoyer au serveur pour vous abonner à tous les [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) dans le dossier boîte de réception à l’aide de l' [opération de s’abonner](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). C’est également la demande XML qui envoie de l’API managée EWS lors de l’abonnement aux notifications de type pull à l’aide de la méthode [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . 
  
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

L’exemple XML suivant montre le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) qui est envoyé à partir du serveur au client en réponse à la requête d’opération **s’abonner** . L’inclusion de la valeur NoError pour l’élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) signifie que l’abonnement a été créé avec succès. L’élément [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifie l’abonnement de notification sur le serveur. L’élément [filigrane](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) représente un signet dans la file d’attente des événements de boîte aux lettres. 
  
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

Après avoir créé l’abonnement, vous pouvez désormais obtenir les événements à l’aide du **SubscriptionId** qui est renvoyé dans le message **SubscribeResponse** . 
  
## <a name="get-pull-notifications-by-using-ews"></a>Obtenir des notifications de type pull à l’aide de EWS
<a name="bk_getpull"> </a>

L’exemple XML suivant montre le message de demande [d’opération GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) est envoyé à partir du client sur le serveur pour obtenir des notifications pour le [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) qui est renvoyé dans le message [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . Pour la première demande **GetEvents** , utilisez le [filigrane](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retourné dans la réponse de **s’abonner** . Pour les demandes **GetEvents** suivantes, utilisez le dernier **filigrane** qui a été retournée dans la demande **GetEvents** précédente. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

L’exemple XML suivant montre le message de réponse **GetEvents** qui est envoyé à partir du serveur au client. Chaque réponse **GetEvents** consacrée des informations sur un ou plusieurs événements. Un **filigrane** est renvoyé pour chaque événement. Le dernier **filigrane** doit être enregistré et utilisé dans la demande **GetEvents** suivante. Si aucun événement magasin n’ont été effectuées depuis la dernière demande **GetEvents** , un événement d’état est retourné. 
  
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

Après avoir reçu un événement à partir du serveur, [synchroniser les modifications sur le client](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Utilisez l' [opération Annuler l’abonnement](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) à la fin de l’abonnement avec le serveur lors de l’abonnement n’est plus nécessaire. 
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_nextsteps"> </a>

Une fois que vous avez reçu les notifications, vous pouvez [synchroniser la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [synchroniser le contenu du dossier qui a été modifiée](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

