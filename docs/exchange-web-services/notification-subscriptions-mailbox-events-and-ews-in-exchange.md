---
title: Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Découvrez les abonnements à des notifications et les événements de boîte aux lettres dans les services EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 2a99b1922e021a8f5f221381d7f2965c3e1ab504
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459353"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange

Découvrez les abonnements à des notifications et les événements de boîte aux lettres dans les services EWS dans Exchange.
  
Vous pouvez utiliser l'API managée des services EWS et les services web Exchange (EWS) pour vous abonner et recevoir des notifications lorsque des événements se produisent dans une boîte aux lettres, ou dans un ou plusieurs des dossiers d'une boîte aux lettres. Trois types d'abonnements sont disponibles : notifications de diffusion en continu, notifications de type pull et notifications Push. Chacun de ces types d'abonnements utilise différentes techniques pour recevoir ou récupérer les notifications.
  
## <a name="getting-notifications---what-are-my-options"></a>Obtenir des notifications - quelles sont les options dont je dispose ?
<a name="bk_notiftypes"> </a>

EWS inclut trois types d'abonnements qui fonctionnent indépendamment pour informer le client de modifications sur le serveur. Quel que soit le type d'abonnement choisi, en fin de compte, vous aurez accès aux mêmes événements de notification - tout dépend de comment vous les obtenez.
  
**Tableau 1. Types d'abonnements**

|**Option**|**Description**|**Me convient-il ?**|
|:-----|:-----|:-----|
|Notifications de diffusion en continu  <br/> |Notifications envoyées par le serveur via une connexion qui reste ouverte pendant une période de temps spécifiée.  <br/> |Les notifications de diffusion en continu sont généralement recommandées pour la plupart des applications. Elles sont semblables aux notifications Push et offrent le meilleur des deux mondes. Une fois que vous avez établi votre abonnement aux notifications, la connexion reste ouverte pendant 30 minutes pour permettre au serveur de renvoyer les notifications au client. Vous n 'avez pas à demander de mises à jour, comme vous le feriez avec un abonnement par extraction, et vous n'avez pas à créer d'application d'écouteur de service web, comme vous le feriez avec un abonnement Push.  <br/> |
|Notifications de type pull  <br/> |Notifications qui sont demandées (ou extraites) par le client.  <br/> |Les notifications de type pull sont généralement plus appropriées pour les clients à faible couplage, lorsque le client n'est pas connecté au réseau de manière fiable. Les notifications de type pull peuvent créer un trafic excessif entre le client et le serveur car le client envoie des demandes fréquentes au serveur pour récupérer des notifications, et toutes les demandes n'entraînent pas des notifications récupérées.  <br/> |
|Notifications push  <br/> |Notifications envoyées (ou poussées) par le serveur vers un service web côté client via une adresse de rappel.  <br/> |En règle générale, les notifications Push fournissent une latence de notification plus faible que les notifications pull et sont adaptées aux clients à couplage étroit auxquels le serveur dispose d'un accès fiable, et il est possible d'accéder au client par le biais d'une adresse IP. Toutefois, les notifications Push ont été laissées de côté depuis l'arrivée des notifications de diffusion en continu dans Exchange 2010. Si possible, nous vous recommandons d'utiliser des notifications de diffusion en continu à la place des notifications Push par la suite. Les notifications Push exigent que vous écriviez une application d'écouteur vers laquelle les notifications sont envoyées. Cela a un léger avantage sur les notifications pull dans la mesure où cela permet de réduire le trafic réseau, mais cela ajoute de la surcharge car une application distincte est requise.  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>À quels événements EWS puis-je m’abonner ?
<a name="bk_eventtypes"> </a>

Les types d'événements EWS auxquels les clients peuvent s'abonner sont définis par l'énumération [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) pour l'API managée EWS ou l'élément [EventType](https://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx) pour EWS. Les événements EWS suivants sont disponibles pour l'abonnement : 
  
- NewMail : un nouveau message est arrivé dans la boîte de réception.
    
- Deleted : un message a été supprimé définitivement de la boîte de réception. Pour en savoir plus sur les notifications des éléments supprimés, voir [Suppression d'éléments à l'aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md) et [Extraction des notifications pour les événements liés à la suppression des boîtes aux lettres EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md).
    
- Modified : un élément ou un dossier a été modifié.
    
- Moved : un élément ou un dossier a été déplacé. 
    
- Copied : un élément ou un dossier a été copié.
    
- Created : Un élément ou un dossier a été créé. 
    
- FreeBusyChanged : les informations de disponibilité d'un utilisateur a été modifiées.
    
Un autre type d'événement EWS, l'événement Status, est défini par l'élément [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx), mais vous ne vous abonnez pas à cet événement. Au lieu de cela, il est envoyé par le serveur pour vérifier l'état du client pour les notifications Push et de diffusion en continu uniquement. Le client doit répondre aux besoins de cet événement ou le client expirera. 
  
Une seule action de l'utilisateur entraîne souvent la création de plusieurs notifications. Pour illustrer cela, la figure suivante illustre quelques scénarios courants et les notifications créées pour chacun d'eux. Les paramètres du client ont un impact sur les notifications reçues, donc il ne s'agit pas d'une liste exhaustive de toutes les options de configuration et des notifications qui en résultent.
  
**Figure 1. Types d'événements renvoyés par les abonnements à des notifications**

![Tableau illustrant les notifications envoyées dans des scénarios utilisateur courants, tels que la réception d’un nouveau message électronique, la création d’un dossier, le déplacement d’un dossier, etc.](media/Exchange2013_Notifications_Events.png)
  
La Figure 1 simplifie le processus de notification. En réalité, plusieurs notifications (même plusieurs notifications du même type) peuvent être créées pour une seule action de l'utilisateur. Par exemple, dans le cas d'une opération de déplacement de dossier, trois événements de dossier sont créés : un pour le dossier en cours de modification, un pour l'ancien dossier parent et un pour le nouveau dossier parent. Étant donné qu'un grand nombre d'événements peut être déclenché pour une seule opération, nous vous recommandons de [générer un délai d'attente de quelques secondes dans vos opérations de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices), afin d'effectuer la synchronisation uniquement lorsque l'action est terminée, plutôt qu'en cours d'opération.
  
Il est également important de savoir que les paramètres de configuration choisis par chaque utilisateur affectent les notifications qui sont créées. Par exemple, les données de disponibilité de certains utilisateurs sont mises à jour automatiquement et l'événement FreeBusyChanged est créé à la réception d'une nouvelle demande de réunion, même avant d'avoir lu l'élément. Pour d'autres utilisateurs, les données de disponibilité ne sont pas mises à jour et l'événement FreeBusyChanged n'est pas créé tant que la réunion n'a pas été acceptée. Ces paramètres peuvent avoir un impact considérable sur les notifications créées par le serveur.
  
## <a name="how-do-ews-notifications-work"></a>Comment fonctionnent les notifications EWS ?
<a name="bk_howwork"> </a>

Les notifications EWS sont gérées par abonnement. En règle générale il existe un abonnement par boîte aux lettres et, dans l'abonnement à la boîte aux lettres, vous pouvez vous abonner à une partie ou à l'intégralité des dossiers. Vous choisissez le type de notification auquel vous souhaitez vous abonner (diffusion en continu, pull ou Push) et le type d'événement que vous souhaitez recevoir (NewMail, Created, Deleted, Modified, etc.) puis vous créez un abonnement. Les événements EWS sont ensuite envoyés de manière asynchrone du serveur de boîte aux lettres au client. (Leçon d'histoire : les événements sont synchrones dans Exchange 2007, et les événements sont stockés sur le serveur d'accès au client dans Exchange 2010, mais pas plus !).
  
La manière dont les notifications sont envoyées au client varie selon le type d'abonnement. Cette section décrit le fonctionnement de chaque type d'abonnement de façon plus détaillée.
  
### <a name="ews-streaming-notifications"></a>Notifications de diffusion en continu EWS
<a name="bk_streamnotif"> </a>

Les notifications de diffusion en continu reposent sur une demande GET en attente sur le serveur pour maintenir une connexion d'abonnement de diffusion en continu ouverte, afin que tous les événements qui se produisent lorsque la connexion est active soient diffusés en continu au client immédiatement. Plusieurs notifications peuvent être envoyées au cours d'une seule connexion et la connexion reste ouverte jusqu'à l'expiration de l'intervalle, ou pendant une période maximale de 30 minutes. Après expiration de la connexion, le client renvoie la demande GET en attente. La Figure 2 illustre le fonctionnement des abonnements de diffusion en continu et des notifications de diffusion en continu.
  
**Figure 2. Vue d'ensemble des notifications de diffusion en continu**

![Illustration présentant le fonctionnement des notifications de diffusion en continu. Pour les configurer : 1. Abonnez-vous, 2. Ouvrez une connexion, 3. Attendez des événements, 4. Recevez des événements, puis répétez les étapes 3 et 4, 5. Fermez ou conservez la connexion, 6. Annulez l’abonnement ou délai d’expiration.](media/Exchange2013_Notifications_StreamSub.png)
  
Pour plus d'informations sur la création de notifications de diffusion en continu, voir [Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-pull-notifications"></a>Notifications de type pull EWS
<a name="bk_pullnotif"> </a>

Les notifications de type pull reposent sur le client qui fait la demande de notifications sur un intervalle qu'il gère. Cela peut entraîner des réponses GetEvents sans notifications. La Figure 3 illustre le fonctionnement des abonnements et des notifications de type pull.
  
**Figure 3. Vue d'ensemble des notifications de type pull**

![Illustration présentant le fonctionnement des notifications de type pull : 1. Abonnez-vous, 2. Envoyez GetEvents, 3. Recevez une réponse, puis répétez les étapes 2 et 3, 4. Fermez ou conservez la connexion, 5. Annulation de l’abonnement ou délai d’expiration.](media/Exchange2013_Notifications_PullSub.png)
  
Pour plus d'informations sur la création des notifications de type pull, voir [Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-push-notifications"></a>Notifications Push EWS
<a name="bk_pushnotif"> </a>

Les notifications Push reposent sur le serveur qui renvoie les notifications au client. Le trafic existe uniquement s'il existe une notification. La Figure 4 illustre le fonctionnement des abonnements et des notifications Push.
  
**Figure 4. Vue d'ensemble des notifications Push**

![Illustration présentant le fonctionnement des notifications push. Pour les configurer : 1. Créez un détecteur, 2. Abonnez-vous, 3. Attendez les événements, 4. Recevez des événements, 5. Envoyez la réponse « OK », puis répétez les étapes 3, 4 et 5, 6. Annulez l’abonnement ou délai d’expiration.](media/Exchange2013_Notifications_PushSub.png)

Si vous utilisez des [notifications Push avec Exchange 2010](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx), envisagez de mettre votre application à niveau pour [utiliser des notifications de diffusion en continu](https://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5). Ainsi, vous n'avez pas besoin d'une application distincte pour recevoir les événements.

  
## <a name="how-do-i-subscribe-to-notifications"></a>Comment s’abonner à des notifications ?
<a name="bk_notifoperations"> </a>

Selon le type d'abonnement que vous souhaitez créer, vous disposez de plusieurs options pour vous abonner à des notifications.
  
**Tableau 2. Opérations et méthodes permettant de s'abonner à des notifications**

|**Type d'abonnement**|**Opération EWS**|**Méthodes d'API managée EWS**|**Fonction**|
|:-----|:-----|:-----|:-----|
|Diffusion en continu  <br/> |[Opération d'abonnement](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.BeginSubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.BeginSubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.SubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |Crée une demande pour s’abonner aux notifications de diffusion en continu.  <br/> |
|Pull  <br/> |[Opération d'abonnement](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.BeginSubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.BeginSubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.SubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Crée une demande pour s’abonner aux notifications de type pull.  <br/> |
|Push  <br/> |[Opération d'abonnement](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Méthode surchargée ExchangeService.BeginSubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Méthode surchargée ExchangeService.BeginSubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Méthode surchargée ExchangeService.SubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Méthode surchargée ExchangeService.SubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Crée une demande pour s’abonner aux notifications Push.  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>Comment obtenir des événements EWS ?
<a name="bk_getevents"> </a>

Une fois que l’abonnement est créé, la façon dont les événements réels sont envoyés au client dépend du type d’abonnement. 
  
Pour les notifications de diffusion en continu, une connexion d’abonnement de diffusion en continu doit être créée puis l’abonnement est ajouté à la connexion. Vous pouvez en savoir plus sur ce processus dans [Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Pour les notifications de type pull, l’objet de l’abonnement a été initialisé lors de la création de l’abonnement. Par conséquent, il vous suffit d’appeler l’opération ou la méthode **GetEvent** pour récupérer les événements à partir du serveur. Vous pouvez en savoir plus sur ce processus dans [Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Le tableau suivant répertorie les opérations et les classes nécessaires pour récupérer des événements. 
  
**Tableau 3. Éléments et classes pour créer une connexion et obtenir des événements**

|**Type d'abonnement**|**Opération EWS**|**Méthode d'API managée EWS**|**Fonction**|
|:-----|:-----|:-----|:-----|
|Diffusion en continu  <br/> |[Opération de GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |[Méthode StreamingSubscriptionConnection.AddSubscription](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |Crée une demande GET en attente sur le serveur, à laquelle une réponse est donnée lorsque des événements se produisent.  <br/> |
|Pull  <br/> |[Opération de GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |[Méthode PullSubscription.GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |Obtient des événements de notification de type pull à partir du serveur.  <br/> |
|Push  <br/> |Non applicable.  <br/> |Non applicable  <br/> |Les notifications Push sont envoyées automatiquement à l'écouteur de service web (l'URL de rappel spécifiée dans la demande d'abonnement). Aucune opération ni méthode supplémentaire ne doit être appelée.  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>Comment résilier des abonnements à des notifications ?
<a name="bk_notifunsubscribe"> </a>

Le tableau suivant répertorie les différentes façons de résilier chaque type d’abonnement.
  
**Tableau 4. Opérations et méthodes de résiliation d'abonnement aux notifications**

|**Type d'abonnement**|**EWS**|**API managée EWS**||
|:-----|:-----|:-----|:-----|
|Diffusion en continu  <br/> |[Opération de résiliation d'abonnement](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Méthode StreamingSubscription.BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Méthode StreamingSubscription.EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Méthode StreamingSubscription.Unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Pull  <br/> |[Opération de résiliation d'abonnement](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Méthode PullSubscription.BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Méthode PullSubscription.EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Méthode PullSubscription.Unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Push  <br/> |Renvoie **Unsubscribe** dans l'élément [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) de [SendNotificationResponseMessage](https://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) <br/> |Non applicable. Laissez plutôt expirer l'abonnement.  <br/> ||
   
Autrement, vous pouvez laisser expirer chacun des abonnements. 
  
**Tableau 5. Délais d'expiration de l'abonnement**

|**Type d'abonnement**|**Valeur du délai d'expiration dans EWS**|**Valeur du délai d'expiration dans l'API managée EWS**|**Gestion des délais d'expiration**|
|:-----|:-----|:-----|:-----|
|Diffusion en continu  <br/> |Élément [ConnectionTimeout](https://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx)  <br/> | Paramètre  *lifetime*  de la méthode [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) constructor  <br/> |Pour l'API managée EWS, une fois le délai d'expiration passé, l'événement [OnDisconnect](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx) se produit. Si la méthode [StreamingSubscriptionConnection.Open](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) n'est pas appelée, la connexion est fermée.  <br/> Pour EWS, une fois le délai expiration écoulé, le message [GetUserConfigurationResponse](https://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) renvoie une valeur [ConnectionStatus](https://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) Closed.  <br/> |
|Pull  <br/> |Élément [Timeout](https://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx)  <br/> | Paramètre  *timeout*  de la méthode [SubscribeToPullNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  <br/> |Une fois que le délai d’expiration s’est écoulé, le serveur supprime l’abonnement.  <br/> |
|Push  <br/> |Élément [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)  <br/> | Paramètre  *frequency*  de la méthode [SubscribeToPushNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  <br/> |Si le serveur ne reçoit pas de réponse à une notification Push ou à un statut ping, il réessaie d'envoyer la notification plusieurs fois avant de cesser d'envoyer les notifications. Pour plus d'informations, voir [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx).  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>Est-il possible de limiter les abonnements ?
<a name="bk_limitsubs"> </a>

Dans un déploiement local, vous pouvez limiter le nombre d'abonnements par utilisateur avec le [paramètre de limitation EwsMaxSubscriptions](ews-throttling-in-exchange.md) de la stratégie de limitation. Cette stratégie peut être appliquée à tous les utilisateurs ou à des utilisateur spécifiques uniquement. La stratégie de limitation **EwsMaxSubscriptions** n'est pas configurable pour Exchange Online. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_limitsubs"> </a>

- [Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
- [Référence des services web pour Exchange](../web-service-reference/web-services-reference-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
- [Exemple d'application de notification Push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

