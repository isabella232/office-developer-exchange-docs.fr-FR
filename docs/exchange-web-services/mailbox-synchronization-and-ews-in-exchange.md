---
title: Synchronisation de la boîte aux lettres et les services EWS d’Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: decf1eee-9743-44f3-9333-b3a01af3683e
description: Découvrez comment fonctionne la synchronisation de la boîte aux lettres lorsque vous utilisez EWS pour accéder à Exchange.
ms.openlocfilehash: 7bca2f7b754dcceee99e4bc24519f6e4f6423ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754987"
---
# <a name="mailbox-synchronization-and-ews-in-exchange"></a>Synchronisation de la boîte aux lettres et les services EWS d’Exchange

Découvrez comment fonctionne la synchronisation de la boîte aux lettres lorsque vous utilisez EWS pour accéder à Exchange.
  
EWS dans Exchange utilise deux types de synchronisation pour extraire le contenu de la boîte aux lettres et les modifications apportées au contenu de la boîte aux lettres :
  
- Synchronisation des dossiers
    
- Synchronisation de l’élément
    
Dans cet article, vous découvrirez les types de synchronisation, comment fonctionne la synchronisation, les modèles de conception de la synchronisation et meilleures pratiques de la synchronisation.
  
## <a name="folder-and-item-synchronization"></a>Synchronisation des dossiers et éléments
<a name="bk_typesofsyncs"> </a>

Synchronisation de dossiers à synchroniser une structure de dossiers, ou la hiérarchie de dossiers. Option de synchronisation permet de synchroniser les éléments dans un dossier. Lorsque vous synchronisez les éléments, vous devez synchroniser indépendamment de chaque dossier dans la boîte aux lettres. Vous pouvez utiliser EWS ou l’API managée EWS dans votre application pour implémenter le dossier et la synchronisation d’élément.
  
**Le tableau 1. Opérations EWS et méthodes d’API managées pour la synchronisation des dossiers et des éléments**

|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
L’étendue de la synchronisation qui se produit est différente selon qu’il soit un initial ou une synchronisation en cours, comme suit :
  
- Synchronisation initiale de synchroniser tous les dossiers ou les éléments sur le serveur au client. Après la synchronisation initiale, le client a un état de synchronisation qu’il stocke des synchronisations ultérieures. L’état de synchronisation représente toutes les modifications sur le serveur que le serveur a communiqué au client.
    
- Synchronisations en cours de synchronisation des éléments ou des dossiers qui ont été ajoutés, supprimés ou modifiés depuis la dernière synchronisation. Le serveur utilise l’état de synchronisation pour calculer les modifications à signaler dans le client au cours de chacune des boucles en cours de synchronisation.
    
Chaque opération ou la méthode de synchronisation renvoie une liste de modifications, pas le dossier en cours ou un message qui a été modifié. Modifications apportées aux éléments et les dossiers sont signalées par les types de modifications suivants :
  
- Créer : Indique qu’un nouvel élément ou un dossier doit être créé sur le client.
    
- Mise à jour — Indique qu’un élément ou un dossier doit être modifiée sur le client.
    
- Supprimer : Indique qu’un élément ou un dossier doit être supprimé sur le client.
    
- ReadStateChange pour EWS ou ReadFlagChange pour l’API managée EWS — indique que l’état de lecture de l’élément a changé, à partir de non lus pour lire ou lecture à non lus.
    
Dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2010 SP2, les éléments et les dossiers sont retournés dans l’ordre de la plus récente à la plus ancienne. Dans les versions précédentes d’Exchange, les éléments et les dossiers sont retournés de la plus ancienne à la plus récente.
  
## <a name="how-does-ews-synchronization-work"></a>Comment fonctionne la synchronisation EWS ?
<a name="bk_howdoesitwork"> </a>

En résumé, si vous effectuez une synchronisation une boîte aux lettres pour la première fois, vous devez utiliser le processus comme le montre la Figure 1. Bien que vous pouvez utiliser d’autres [modèles de conception de la synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns), nous vous recommandons cette approche pour les applications évolutives.
  
**La figure 1. Modèle de conception de la synchronisation initiale**

![Illustration présentant le modèle de conception de synchronisation initial. Le client appelle SyncFolderHierarchy et Load ou GetItem pour obtenir les dossiers, puis appelle SyncFolderItems et LoadPropertiesForItems ou GetItem pour obtenir les éléments de chaque dossier.](media/Exchange2013_SyncInitial.png)
  
Si vous utilisez un état de synchronisation existant sur le client pour synchroniser une boîte aux lettres, il est recommandé d’implémenter le modèle de conception comme indiqué dans la Figure 2. 
  
**La figure 2. Modèle de conception en cours de synchronisation**

![Illustration présentant le modèle de conception de synchronisation en cours. Un client reçoit une notification, puis appelle SyncFolderHierarchy ou SyncFolderItems ; il obtient les propriétés, puis met à jour le client ou met simplement à jour l’indicateur de lecture sur le client.](media/Exchange2013_Sync_Ongoing.png)
  
## <a name="synchronization-design-patterns"></a>Modèles de conception de la synchronisation
<a name="bk_syncpatterns"> </a>

Vous pouvez utiliser une des deux modèles de conception de la synchronisation dans votre application pour vos boîtes aux lettres de mise à jour : la synchronisation de notification ou l’approche de la synchronisation.
  
Synchronisation de notification, comme illustré dans [la Figure 2](mailbox-synchronization-and-ews-in-exchange.md#bk_howdoesitwork), repose sur l’utilisation des notifications d’alerte du client pour émettre un appel pour les méthodes API managées [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) ou [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) ou la [SyncFolderHierarchy EWS ](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)ou opérations [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) . Ce type de synchronisation est généralement recommandé pour les applications évolutives, mais il ne peut pas être la meilleure approche pour tout le monde. La synchronisation de notification présente l’avantage suivant : 
  
- Les notifications sont optimisées pour réduire les appels vers la base de données Exchange principale. Abonnements et des files d’attente d’événements sont gérés par le serveur de boîtes aux lettres (ou le serveur d’accès Client dans Exchange 2010 et Exchange 2007) ; Toutefois, la gestion des événements et des abonnements utilise moins de ressources que la solution, qui est plus fréquente des appels de synchronisation à la base de données Exchange. En outre, Exchange a spécifiques des [stratégies de limitation](ews-throttling-in-exchange.md) pour les notifications et aux abonnements protéger la consommation des ressources. 
    
Toutefois, il existe également des inconvénients à l’utilisation de la synchronisation de notification :
  
- Les notifications sont BRUITEES, car la plupart des scénarios impliquant des notifications multiples lors de l’objectif d’un utilisateur. Ceci est particulièrement vrai du dossier calendrier. Par exemple, lors de la réception d’une demande de réunion unique, plusieurs notifications d’éléments et dossiers sont créées, y compris une notification pour créer l’élément et l’autre pour modifier l’élément. Pour atténuer cet inconvénient consiste à créer un délai de quelques secondes à votre appel [charge](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.load%28v=exchg.80%29.aspx), [LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx), [GetItem](http://msdn.microsoft.com/en-us/library/exchange/aa565934%28v=exchg.150%29.aspx.aspx)ou [GetFolder](http://msdn.microsoft.com/en-us/library/exchange/aa580274%28v=exchg.150%29.aspx.aspx) . Dans le cas d’une demande de réunion, si vous avez apporté des appels à l’opération **GetItem** immédiatement, vous devrez peut-être un appel pour créer l’élément et l’autre pour modifier l’élément. Au lieu de cela, en retardant l’appel, vous pouvez appeler une fois l’opération de **GetItem** et apporter des modifications qui régissent la création et la modification de l’élément en même temps. 
    
- Les notifications sont en file d’attente sur le serveur de boîtes aux lettres et les abonnements sont enregistrés sur le serveur de boîtes aux lettres. Si le serveur de boîtes aux lettres qui gère l’abonnement n’est pas disponible, vous perdez les notifications de nouveau votre boîte aux lettres ne synchroniser et vous devrez réabonner aux notifications.
    
- Vous devez planifier des stratégies d’atténuation dans le cas où les notifications d’échouent. De cette façon, la deuxième approche, le modèle de conception de la synchronisation uniquement, est plus robuste que la synchronisation basée sur une notification, car elle nécessite uniquement que le client de mettre à jour l’état de synchronisation : aucun problème avec affinité pour le serveur de boîtes aux lettres gestion de l’abonnement.
    
Si implémentée comme recommandé, le modèle de conception d’abonnement basé sur la notification s’appuie sur : 
  
- Notifications pour déterminer *quand* les données modifiées. 
    
- L' API managée EWS **SyncFolderHierarchy** ou méthodes **SyncFolderItems** , ou le EWS **SyncFolderHierarchy** ou opérations **SyncFolderItems** pour déterminer *quel* modifié, optimiser le nombre d’événements de synchronisation renvoyé. A un nouvel élément créé, mis à jour ou supprimé ? C’est tout ce que vous devez connaître à partir de ces méthodes, n’ont besoin pour la liste des propriétés des modifications. (Ne pas faire une **GetItem** ou un appel de **LoadPropertiesForItems** sur tous les éléments ou des dossiers retournés). 
    
- L’aide des méthodes **de chargement** ou **LoadPropertiesForItems** dans l’API managée EWS, ou de l’opération EWS **GetItem** pour déterminer *comment* les données modifiées et pour récupérer les propriétés à partir du serveur, le cas échéant, organiser des requêtes groupées en fonction de sur la quantité de données qui seront retournés. Elle est suivie une comparaison des propriétés sur le client et ceux simplement renvoyés à partir du serveur et finalement la création, suppression ou modification de l’élément ou un dossier sur le client. 
    
L’approche de synchronisation repose entièrement sur les méthodes **SyncFolderItems** et API managées **SyncFolderHierarchy** , ou **SyncFolderHierarchy** ou EWS **SyncFolderItems** opérations que vous pouvez appeler soit en permanence, ou en tant qu’un événement chronométré. Il existe des avantages et inconvénients ainsi que cette option. L’approche de la synchronisation est plus robuste, car l’état de synchronisation est stocké sur le client au niveau de la boîte aux lettres et une relation unique entre l’état de synchronisation et tout le serveur de boîtes aux lettres qui gère l’abonnement de notification n’est pas requis. L’approche de la synchronisation puisse résister à un basculement de la boîte aux lettres en raison de son indépendance à partir du serveur de boîtes aux lettres. Toutefois, l’approche de la synchronisation augmente la latence pour l’utilisateur, car les éléments sont synchronisés sur une base chronométrée ou intermittente — pas dans l’arrivée en temps réel. Cette approche est également plus coûteuse, car vous êtes des appels à la base de données Exchange lorsqu’il est possible qu’aucune modification ne se sont produites. 
  
## <a name="synchronization-best-practices"></a>Meilleures pratiques de la synchronisation
<a name="bk_bestpractices"> </a>

Pour les applications hautement évolutives, nous vous recommandons d’appliquer les meilleures pratiques suivantes pour synchroniser les boîtes aux lettres dans votre application :
  
- Lors de l’appel de la méthode API managées **SyncFolderItems** ou **SyncFolderHierarchy** d’utiliser la valeur _IdOnly_ pour le paramètre _propertySet_ , ou lorsque vous utilisez le EWS **SyncFolderHierarchy** ou **SyncFolderItems** opérations utilisent la valeur **IdOnly** pour la valeur [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) pour réduire les appels vers la base de données Exchange. Les propriétés plus vous demander dans le jeu de propriétés du **SyncFolderItems** ou **SyncFolderHierarchy** appel, le principal plusieurs appels sont créés. Un nouvel appel RPC est effectué pour chaque valeur de la propriété demandée, tandis que qu’un seul appel de procédure distante est effectué pour récupérer tous les **numéros d’objet** pour une demande - quel que soit le nombre de résultats pour le rapport. Pour une demande **IdOnly** les résultats de l’appel d’une base de données, tandis que les résultats d’une demande de conteneur de propriété pour l’objet et l’expéditeur dans trois appels de base de données : un pour l' **objet**, un pour l' **expéditeur**et un pour l' **ID d’élément**.
    
- N’appelez pas les méthodes API managées **charge** ou **LoadPropertiesForItems** , ou EWS **GetItem** ou opérations **GetFolder** , sur chaque élément dans une réponse de la synchronisation. Au lieu de cela, analyser les résultats ; Rechercher les modifications qui ne nécessitent pas toutes les propriétés à récupérer, comme lire les modifications de l’état. Si une réponse inclut un changement d’état de lecture, simplement mettre à jour l’indicateur sur le client et vous avez terminé ; pas nécessaire pour obtenir toutes les propriétés de l’élément. Et assurez-vous que vous éviter des efforts en apportant des modifications à l’origine à partir du même client. Par exemple, si la réponse de la synchronisation inclut la suppression d’un élément et que la suppression s’est produite sur le client local, vous n’avez pas besoin supprimer le message à nouveau ou obtenir toutes les propriétés de cet élément. 
    
- Éviter d’obtention limitées, en procédant comme suit :
    
  - Lorsque vous appelez la méthode API managées **LoadPropertiesForItems** ou l’opération EWS **GetItem** pour obtenir les éléments d’un lot, procédez comme lot pas trop d’éléments dans votre demande ; dans le cas contraire, vous pouvez obtenir [limitées](ews-throttling-in-exchange.md). Nous vous conseillons d’inclure 10 éléments par lot.
    
  - Ne faites pas trop de requêtes dans un temps trop court. Seront également entraîner la limitation et augmenter le temps de réponse, plutôt que de raccourcir. 
    
  - Si vous sont traitement par lots des éléments, tous les éléments ayant les mêmes valeurs pour les attributs **Id** et **ChangeKey** de l’élément [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du lot. 
    
  - Si vous obtenir limitées, arrêter l’envoi de demandes. Renvoi des demandes système prolonger l’effort de récupération. Au lieu de cela, attendez que l’heure d’expiration d’interruption, puis tentez à nouveau d’envoyer vos demandes de synchronisation.
    
- Selon le type d' [événement de notification](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_eventtypes) reçue : 
    
  - Pour les événements **NewMail** ou **modifié** , appeler la méthode API managées **SyncFolderItems** ou l’opération EWS **SyncFolderItems** parce que les notifications ne fournissent pas un **ChangeKey**et notifications n’appellent pas état de lecture modifications apportées.
    
  - Pour les événements **supprimés** , si l’abonnement de notification était active avant la synchronisation précédente, supprimez simplement l’événement localement. Il est inutile d’appeler la méthode API managées **SyncFolderItems** ou l’opération EWS **SyncFolderItems** immédiatement après la suppression. 
    
  - Si un événement de **modification** a été provoqué par une modification de l’état « lu », ne pas appeler la méthode API managées **LoadPropertiesForItems** ou l’opération EWS **GetItem** , il suffit de modifier l’indicateur sur l’élément. 
    
- Lors de la synchronisation des données de calendrier, procédez comme suit :
    
  - Utilisez une approche similaire à la synchronisation de notification. Car **SyncFolderItem** n’inclut pas la logique du calendrier, utilisez la méthode d’API managées [FindAppointments](http://msdn.microsoft.com/en-us/library/dd633767%28v=exchg.80%29.aspx) , ou l' EWS [FindItem opération](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec l’élément [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) pour afficher les rendez-vous entre deux dates, puis Appelez la méthode API managées **LoadPropertiesForItems** ou l’opération EWS **GetItem** pour récupérer les propriétés d’élément pour l’élément de calendrier. 
    
  - Pas interroger à l’aide de la méthode API managées **FindAppointments** ou l’opération EWS **FindItem** avec un élément **CalendarView** . 
    
- Lors de la synchronisation des dossiers de recherche :
    
  - Utilisez une approche similaire à la synchronisation de notification. 
    
  - Utilisation des notifications pour déterminer quand les données sont modifiées.
    
  - Car vous ne pouvez pas utiliser **SyncFolderItem** dans un dossier de recherche, utilisez une méthode de l' API managée EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) trié et paginé, ou une opération EWS **FindItem** avec l’ensemble d’éléments [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) et [SortOrder](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , pour déterminer ce qui est modifié. 
    
  - Utilisez la méthode API managées **LoadPropertiesForItems** ou l’opération EWS **GetItem** pour récupérer des données. 
    
## <a name="filtered-synchronization"></a>Synchronisation filtrée
<a name="bk_filteredsync"> </a>

La méthode API managées **SyncFolderItems** et l’opération EWS **SyncFolderItems** permettent d’ignorer les éléments spécifiques, en fonction de leurs numéros d’objet, en définissant le paramètre _ignoreItemIds_ dans l’API managée EWS ou [case à cocher Ignorer](http://msdn.microsoft.com/library/7789eec5-ceec-43f2-84d5-d0d15b734076%28Office.15%29.aspx) élément dans EWS. Cela est idéal lorsque, par exemple, personnes commencent à répondre à tous dans un message électronique envoyé à tout le monde. 
  
Vous pouvez vous demander, puis-je filtrer mes notifications (et par conséquent seulement déclencher la synchronisation) si vous modifient des propriétés spécifiques ? Bien que cela semble raisonnable, étant donné que les abonnements aux notifications sont basées sur le type de modification (créer, mettre à jour, supprimer), et pas la propriété mis à jour, vous ne pouvez pas filtrer les notifications de cette manière. Vous pouvez au lieu de cela, procédez comme suit :
  
- Utiliser le modèle de conception d’abonnement basé sur la notification.
    
- Appeler les API managées **SyncFolderItems** et méthodes **SyncFolderHierarchy** se succèdent en alternance avec le paramètre _propertySet_ _IdOnly_ la valeur pour rendre votre état de synchronisation actuel. Ou si vous utilisez EWS, appeler les **SyncFolderHierarchy** et opérations **SyncFolderItems** à plusieurs reprises avec la valeur **BaseShape** **IdOnly**. 
    
- Ignorer la réponse (ne pas analyser ou effectuer des comparaisons de propriété).
    
- Utilisez la méthode API managées **FindItems** ou l’opération EWS **FindItem** et tri et page pour préremplir les éléments dans l’étendue filtrée qui vous intéressent. 
    
- Utilisez votre état de synchronisation pour continuer à appeler la méthode API managées **SyncFolderItems** ou l’opération EWS **SyncFolderItems** , mais uniquement surveiller les changements apportés dans l’ensemble filtré d’élément. Si les nouveaux éléments sont créés, vous devrez voir si ces éléments sont dans votre étendue filtrée. 
    
## <a name="in-this-section"></a>Dans cette section
<a name="bk_filteredsync"> </a>

- [Synchroniser les dossiers à l’aide de EWS dans Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Synchroniser des éléments à l’aide de EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Méthode SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx)
    
- [Méthode SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)
    
- [Opération SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)
    
- [Opération SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)
    

