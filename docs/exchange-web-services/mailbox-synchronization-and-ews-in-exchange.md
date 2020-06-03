---
title: Synchronisation de la boîte aux lettres et les services EWS d'Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: decf1eee-9743-44f3-9333-b3a01af3683e
description: Découvrez le fonctionnement de la synchronisation des boîtes aux lettres lorsque vous utilisez EWS pour accéder à Exchange.
localization_priority: Priority
ms.openlocfilehash: 5dc700c7feb9fce6121a27ee73fc1a58e88e643a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456258"
---
# <a name="mailbox-synchronization-and-ews-in-exchange"></a>Synchronisation de la boîte aux lettres et les services EWS d'Exchange

Découvrez le fonctionnement de la synchronisation des boîtes aux lettres lorsque vous utilisez EWS pour accéder à Exchange.
  
EWS dans Exchange utilise deux types de synchronisation pour récupérer le contenu des boîtes aux lettres et les modifications apportées au contenu des boîtes aux lettres :
  
- Synchronisation de dossiers
    
- Synchronisation des éléments
    
Dans cet article, vous découvrirez les deux types de synchronisation, le fonctionnement de la synchronisation, les modèles de conception de la synchronisation et les meilleures pratiques en matière de synchronisation.
  
## <a name="folder-and-item-synchronization"></a>Synchronisation des éléments et des dossiers
<a name="bk_typesofsyncs"> </a>

La synchronisation de dossiers synchronise une structure de dossiers ou une hiérarchie de dossiers. La synchronisation d’éléments synchronise les éléments dans un dossier. Lorsque vous synchronisez des éléments, vous devez synchroniser chaque dossier de la boîte aux lettres indépendamment. Vous pouvez utiliser EWS ou l’API managée EWS dans votre application pour implémenter la synchronisation des dossiers et des éléments.
  
**Tableau 1. Opérations EWS et méthodes de l’API managée EWS pour la synchronisation des dossiers et des éléments**

|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
L’étendue de la synchronisation qui se produit diffère selon qu’il s’agit d’une synchronisation initiale ou d’une synchronisation en cours, comme suit :
  
- Une synchronisation initiale synchronise tous les dossiers ou éléments sur le serveur avec le client. Après la synchronisation initiale, le client a un état de synchronisation qu’il stocke pour les synchronisations futures. L’état de synchronisation représente toutes les modifications sur le serveur que le serveur a communiqué au client.
    
- Synchronisations en cours synchronisez tous les éléments ou dossiers qui ont été ajoutés, supprimés ou modifiés depuis la synchronisation précédente. Le serveur utilise l’état de synchronisation pour calculer les modifications apportées au client lors de chacune des boucles de synchronisation en cours.
    
Chaque opération ou méthode de synchronisation renvoie une liste de modifications, pas le dossier ou le message réel qui a été modifié. Les modifications apportées aux éléments et aux dossiers sont signalées au moyen des types de modifications suivants :
  
- Créer — indique qu’un nouvel élément ou dossier doit être créé sur le client.
    
- Update : indique qu’un élément ou un dossier doit être modifié sur le client.
    
- Supprimer : indique qu’un élément ou un dossier doit être supprimé sur le client.
    
- ReadStateChange pour EWS ou ReadFlagChange pour l’API managée EWS : indique que l’état de lecture de l’élément a changé, qu’il soit de non lu ou lu à non lu.
    
Dans Exchange Online, Exchange Online dans le cadre d’Office 365 et versions d’Exchange à partir d’Exchange 2010 SP2, les éléments et les dossiers sont renvoyés dans l’ordre du plus récent au plus ancien. Dans les versions précédentes d’Exchange, les éléments et les dossiers sont retournés du plus ancien au plus récent.
  
## <a name="how-does-ews-synchronization-work"></a>Comment fonctionne la synchronisation EWS ?
<a name="bk_howdoesitwork"> </a>

En bref, si vous synchronisez une boîte aux lettres pour la première fois, utilisez le processus comme illustré dans la figure 1. Bien que vous puissiez utiliser d’autres [modèles de conception de synchronisation](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns), nous vous recommandons d’utiliser cette approche pour les applications évolutives.
  
**Figure 1. Modèle de conception de la synchronisation initiale**

![Illustration présentant le modèle de conception de synchronisation initial. Le client appelle SyncFolderHierarchy et Load ou GetItem pour obtenir les dossiers, puis appelle SyncFolderItems et LoadPropertiesForItems ou GetItem pour obtenir les éléments de chaque dossier.](media/Exchange2013_SyncInitial.png)
  
Si vous utilisez un état de synchronisation existant sur le client pour synchroniser une boîte aux lettres, nous vous recommandons d’implémenter le modèle de conception comme indiqué dans la figure 2. 
  
**Figure 2. Modèle de conception de la synchronisation continue**

![Illustration présentant le modèle de conception de synchronisation en cours. Un client reçoit une notification, puis appelle SyncFolderHierarchy ou SyncFolderItems ; il obtient les propriétés, puis met à jour le client ou met simplement à jour l’indicateur de lecture sur le client.](media/Exchange2013_Sync_Ongoing.png)
  
## <a name="synchronization-design-patterns"></a>Modèles de conception de la synchronisation
<a name="bk_syncpatterns"> </a>

Vous pouvez utiliser l’un des deux modèles de conception de synchronisation dans votre application pour maintenir vos boîtes aux lettres à jour : la synchronisation basée sur les notifications ou l’approche de synchronisation uniquement.
  
La synchronisation basée sur les notifications, comme illustré à la [figure 2](mailbox-synchronization-and-ews-in-exchange.md#bk_howdoesitwork), s’appuie sur des notifications pour alerter le client à appeler les méthodes [SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) ou [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) de l’API managée EWS, ou les opérations EWS [opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) ou [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) . Ce type de synchronisation est généralement recommandé pour les applications évolutives, mais il n’est peut-être pas la meilleure approche pour tout le monde. La synchronisation basée sur les notifications présente les avantages suivants : 
  
- Les notifications sont optimisées pour réduire les appels à la base de données Exchange principale. Les files d’attente d’événements et les abonnements sont gérés par le serveur de boîtes aux lettres (ou par le serveur d’accès au client dans Exchange 2010 et Exchange 2007); Toutefois, la gestion des événements et des abonnements utilise moins de ressources que l’alternative, ce qui représente des appels de synchronisation plus fréquents à la base de données Exchange. En outre, Exchange possède des [stratégies de limitation](ews-throttling-in-exchange.md) spécifiques pour les notifications et les abonnements, afin de préserver la consommation des ressources. 
    
Toutefois, il existe quelques inconvénients à l’utilisation de la synchronisation basée sur les notifications :
  
- Les notifications sont bruyantes car la plupart des scénarios impliquent plusieurs notifications pour un objectif d’utilisateur. Ceci est particulièrement vrai pour le dossier calendrier. Par exemple, lorsqu’une demande de réunion unique est reçue, plusieurs notifications d’éléments et de dossiers sont créées, y compris une notification pour créer l’élément et une autre pour modifier l’élément. Pour atténuer cet inconvénient, vous pouvez créer un délai de quelques secondes dans votre appel [Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.load%28v=exchg.80%29.aspx), [LoadPropertiesForItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx), [GetItem](https://msdn.microsoft.com/library/exchange/aa565934%28v=exchg.150%29.aspx.aspx)ou [GetFolder](https://msdn.microsoft.com/library/exchange/aa580274%28v=exchg.150%29.aspx.aspx) . Dans le cas d’une demande de réunion, si vous avez effectué des appels à l’opération **GetItem** immédiatement, vous pouvez avoir un appel pour créer l’élément et un autre pour modifier l’élément. Au lieu de cela, en retardant l’appel, vous pouvez appeler l’opération **GetItem** une seule fois et obtenir les modifications qui englobent la création et la modification de l’élément en même temps. 
    
- Les notifications sont mises en file d’attente sur le serveur de boîtes aux lettres et les abonnements sont enregistrés sur le serveur de boîtes aux lettres. Si le serveur de boîtes aux lettres qui gère l’abonnement n’est pas disponible, vous perdez toutes les nouvelles notifications, votre boîte aux lettres ne sera pas synchronisée et vous devrez vous reabonner aux notifications.
    
- Vous devrez planifier des stratégies de minimisation en cas d’échec des notifications. De cette manière, la deuxième approche, le modèle de conception de synchronisation uniquement, est plus résiliente que la synchronisation basée sur les notifications, car elle nécessite uniquement que le client conserve l’état de synchronisation ; il n’y a aucun problème lié à l’affinité avec le serveur de boîtes aux lettres qui gère l’abonnement.
    
Si elle est implémentée comme recommandé, le modèle de conception de l’abonnement basé sur la notification s’appuie sur les éléments suivants : 
  
- Notifications permettant de déterminer *quand* les données ont été modifiées. 
    
- Les méthodes **opérationsyncfolderhierarchy** ou **SYNCFOLDERITEMS** de l’API managée EWS, ou les opérations EWS **opérationsyncfolderhierarchy** ou **SyncFolderItems** pour déterminer *ce qui* a changé, en optimisant le nombre d’événements de synchronisation renvoyés. Un nouvel élément a-t-il été créé, mis à jour ou supprimé ? Tout ce que vous avez besoin de découvrir de ces méthodes, ne vous en faites pas confiance pour la liste des propriétés des modifications. (Ne pas appeler **GetItem** ou **LoadPropertiesForItems** sur tous les éléments ou dossiers renvoyés). 
    
- À l’aide des méthodes **Load** ou **LOADPROPERTIESFORITEMS** dans l’API managée EWS, ou de l’opération de GetItem de la fonction de **GetItem** pour déterminer la *façon dont* les données ont été modifiées et de récupérer les propriétés à partir du serveur si nécessaire, en organisant les requêtes regroupées en fonction de la quantité de données qui seront renvoyées. Elle est suivie d’une comparaison entre les propriétés sur le client et celles qui viennent d’être renvoyées à partir du serveur, et enfin la création, la suppression ou la modification de l’élément ou du dossier sur le client. 
    
L’approche de synchronisation unique repose entièrement sur les méthodes d’API managée EWS **SyncFolderItems** et **opérationsyncfolderhierarchy** , ou sur les opérations EWS **opérationsyncfolderhierarchy** ou **SyncFolderItems** , que vous pouvez appeler en continu ou en tant qu’événement chronométré. Cette option présente également des avantages et des inconvénients. L’approche de synchronisation uniquement est plus résiliente car l’état de synchronisation est stocké sur le client au niveau de la boîte aux lettres et une relation unique entre l’état de synchronisation et tout serveur de boîtes aux lettres qui gère l’abonnement aux notifications n’est pas nécessaire. L’approche de synchronisation peut survivre à un basculement de boîte aux lettres en raison de son indépendance par rapport au serveur de boîtes aux lettres. Toutefois, l’approche de synchronisation augmente la latence de l’utilisateur, car les éléments sont synchronisés à intervalles réguliers ou intermittents, et non en temps réel lorsque les éléments arrivent. Cette approche est également plus coûteuse, car vous effectuez des appels à la base de données Exchange lorsqu’il est possible qu’aucune modification ne se soit produite. 
  
## <a name="synchronization-best-practices"></a>Meilleures pratiques en matière de synchronisation
<a name="bk_bestpractices"> </a>

Pour les applications hautement évolutives, nous vous recommandons d’appliquer les meilleures pratiques suivantes pour synchroniser des boîtes aux lettres dans votre application :
  
- Lors de l’appel de la méthode **SyncFolderItems** ou **OPÉRATIONSYNCFOLDERHIERARCHY** de l’API managée EWS, utilisez la valeur _IdOnly_ pour le paramètre _PropertySet_ , ou lorsque vous utilisez les opérations EWS **opérationsyncfolderhierarchy** ou **SyncFolderItems** utilisez la valeur **IdOnly** pour la valeur [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) afin de réduire les appels à la base de données Exchange. Plus le nombre de propriétés que vous demandez dans le jeu de propriétés de l’appel **SyncFolderItems** ou **opérationsyncfolderhierarchy** , plus les appels back-end sont créés. Un nouvel appel RPC est effectué pour chaque valeur de propriété demandée, alors qu’un seul appel RPC est effectué pour extraire toutes les **ItemIds** pour une demande, quel que soit le nombre de résultats à signaler. Ainsi, une requête **IdOnly** entraîne un appel de base de données, tandis qu’une demande de conteneur de propriétés pour l’objet et l’expéditeur génère trois appels de base de données : un pour l' **objet**, un pour l' **expéditeur**et un pour l' **ItemId**.
    
- N’appelez pas les méthodes **Load** ou **LOADPROPERTIESFORITEMS** de l’API managée EWS, ou les **opérations EWS ou** **GetFolder** , sur chaque élément d’une réponse de synchronisation. Analysez plutôt les résultats ; Recherchez les modifications qui ne nécessitent pas toutes les propriétés à récupérer, comme les modifications de l’état de lecture. Si une réponse inclut un changement d’état de lecture, mettez simplement à jour l’indicateur sur le client et vous avez terminé ; Il n’est pas nécessaire d’obtenir toutes les propriétés d’élément. Et assurez-vous que vous ne dupliquez pas les efforts en effectuant des modifications provenant du même client. Par exemple, si la réponse de synchronisation inclut la suppression d’un élément et que la suppression s’est produite sur le client local, vous n’avez pas besoin de supprimer de nouveau le message ou d’obtenir toutes les propriétés de cet élément. 
    
- Évitez d’être limité en procédant comme suit :
    
  - Lorsque vous appelez la méthode **LoadPropertiesForItems** de l’API managée EWS ou l’opération EWS **GetItem** pour obtenir les éléments dans un lot, ne confondez pas trop d’éléments dans votre demande ; dans le cas contraire, vous pouvez être [limité](ews-throttling-in-exchange.md). Nous vous recommandons d’inclure 10 éléments par lot.
    
  - Ne pas faire trop de demandes trop rapidement. Cela entraînera également une limitation et augmentera le temps de réponse, plutôt que de le raccourcir. 
    
  - Si vous effectuez le traitement par lots des éléments, tous les éléments sont regroupés avec les mêmes valeurs pour les attributs **ID** et **ChangeKey** de l’élément [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . 
    
  - Si vous obtenez des limitations, arrêtez l’envoi de demandes. Les demandes de renvoi vont prolonger l’effort de récupération. Au lieu de cela, patientez jusqu’à ce qu’il expire, puis essayez à nouveau d’envoyer vos demandes de synchronisation.
    
- Selon le type d’événement de [notification](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_eventtypes) reçu : 
    
  - Pour les événements **NewMail** ou **modifié** , appelez la méthode **SyncFolderItems** de l’API managée EWS ou l’opération EWS **SyncFolderItems** car les notifications ne fournissent pas de **ChangeKey**, et les notifications n’appellent pas les modifications de l’état de lecture.
    
  - Pour les événements **supprimés** , si l’abonnement aux notifications était actif avant la synchronisation précédente, supprimez simplement l’événement localement. Il n’est pas nécessaire d’appeler la méthode **SyncFolderItems** de l’API managée EWS ou l’opération EWS **SyncFolderItems** immédiatement après la suppression. 
    
  - Si un événement **modifié** est dû à une modification de l’état de lecture, n’appelez pas la méthode **LOADPROPERTIESFORITEMS** de l’API managée EWS ou l’opération de **GetItem** , il suffit de modifier l’indicateur sur l’élément. 
    
- Lors de la synchronisation des données de calendrier, procédez comme suit :
    
  - Utilisez une approche similaire à la synchronisation basée sur les notifications. Étant donné que **SyncFolderItem** n’inclut aucune logique de calendrier, utilisez la méthode [FINDAPPOINTMENTSPOUR](https://msdn.microsoft.com/library/dd633767%28v=exchg.80%29.aspx) de l’API managée EWS ou l' [opération EWS FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec l’élément [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) pour afficher les rendez-vous entre deux dates, puis appelez la méthode **LoadPropertiesForItems** de l’API managée EWS ou l’opération de **GetItem** EWS pour extraire les propriétés de l’élément de calendrier. 
    
  - Ne pas effectuer d’interrogation à l’aide de la méthode **findappointmentspour** de l’API managée EWS, ni de l’opération EWS **FindItem** avec un élément **CalendarView** . 
    
- Lors de la synchronisation des dossiers de recherche :
    
  - Utilisez une approche similaire à la synchronisation basée sur les notifications. 
    
  - Utilisez les notifications pour déterminer quand les données sont modifiées.
    
  - Étant donné que vous ne pouvez pas utiliser **SyncFolderItem** dans un dossier de recherche, utilisez une méthode [FINDITEMS](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) de l’API managée EWS triée et paginée, ou une opération EWS **FindItem** avec l’ensemble d’éléments [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) et [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , pour déterminer ce qui a été modifié. 
    
  - Utilisez la méthode **LoadPropertiesForItems** de l’API managée EWS ou l’opération de **GetItem** pour extraire des données. 
    
## <a name="filtered-synchronization"></a>Synchronisation filtrée
<a name="bk_filteredsync"> </a>

La méthode **SyncFolderItems** de l’API managée EWS et l’opération EWS **SyncFolderItems** vous permettent d’ignorer des éléments spécifiques, en fonction de leur ItemIds, en définissant le paramètre _ignoreItemIds_ dans l’API managée EWS ou l’élément [ignore](https://msdn.microsoft.com/library/7789eec5-ceec-43f2-84d5-d0d15b734076%28Office.15%29.aspx) dans EWS. Ceci est idéal lorsque, par exemple, des personnes commencent à répondre à tous dans un message électronique envoyé à tous les membres de l’entreprise. 
  
Vous pouvez vous demander s’il est possible de filtrer mes notifications (et par conséquent de déclencher uniquement la synchronisation) si des propriétés spécifiques changent ?. Bien que cela semble raisonnable, étant donné que les abonnements aux notifications sont basés sur le type de modification (Create, Update, Delete) et non sur la propriété en cours de mise à jour, vous ne pouvez pas filtrer les notifications de cette façon. Au lieu de cela, vous pouvez effectuer les opérations suivantes :
  
- Utilisez le modèle de conception de l’abonnement basé sur les notifications.
    
- Appelez de manière répétée les méthodes **SyncFolderItems** et **OPÉRATIONSYNCFOLDERHIERARCHY** de l’API managée EWS avec le paramètre _PropertySet_ défini sur _IdOnly_ pour que votre état de synchronisation soit actif. Ou, si vous utilisez EWS, appelez les opérations **opérationsyncfolderhierarchy** et **SyncFolderItems** à plusieurs reprises, avec la valeur **BaseShape** définie sur **IdOnly**. 
    
- Ignorez la réponse (ne l’analysez pas ou n’effectuez pas de comparaisons de propriétés).
    
- Utilisez la méthode **FindItems** de l’API managée EWS ou l’opération **FindItem** EWS et le tri et la page pour préremplir les éléments de l’étendue filtrée qui vous intéressent. 
    
- Utilisez votre état de synchronisation pour continuer à appeler la méthode **SyncFolderItems** de l’API managée EWS ou l’opération EWS **SyncFolderItems** , mais uniquement surveiller les modifications apportées à l’ensemble d’éléments filtré. Si de nouveaux éléments sont créés, vous devez voir si ces nouveaux éléments se trouvent dans votre portée filtrée. 
    
## <a name="in-this-section"></a>Dans cette section
<a name="bk_filteredsync"> </a>

- [Synchroniser des dossiers à l’aide d’EWS dans Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Synchroniser des éléments à l’aide d’EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Méthode SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx)
    
- [Méthode Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)
    
- [Opération Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)
    
- [Opération SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)
    

