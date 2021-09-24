---
title: Restauration de Exchange bases de données 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Trouvez des informations sur les différentes façons de restaurer vos bases de données Exchange 2013.
ms.openlocfilehash: 522128026bcbef893ce4909174d3fd9a95f1e8a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513275"
---
# <a name="restoring-exchange-2013-databases"></a>Restauration de Exchange bases de données 2013

Trouvez des informations sur les différentes façons de restaurer vos bases de données Exchange 2013. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange inclus dans Exchange Server 2013 offre une certaine flexibilité dans la restauration de vos bases de données Exchange données. En utilisant le rédacteur Exchange dans Exchange 2013, vous pouvez restaurer vos sauvegardes de shadow copy aux emplacements suivants :
  
- Base de données d’origine, que la configuration du chemin d’accès de la base de données ou du fichier journal des transactions ait été modifiée.
    
- Une base de données de récupération.
    
- Toute base de données de production, que le nom complet de la base de données corresponde ou non au nom d’un jeu de sauvegarde VSS.
    
Lorsque votre application de restauration restaure des informations dans la base de données d’origine, les fichiers journaux doivent être restaurés dans le chemin d’accès au répertoire spécifié dans les services de domaine Active Directory (AD DS) pour cette base de données. Si votre application restaure une base de données à un autre emplacement, les fichiers journaux doivent être restaurés dans un dossier nommé **_restoredLogs** situé dans le répertoire des fichiers journaux de base de données. 
  
Lors de la restauration vers un serveur ou une base de données différent de la base de données d’origine, votre application de restauration doit s’assurer que les chemins d’accès au répertoire de base de données fournis au service VSS correspondent à ceux des services AD DS. Vous pouvez utiliser la cmdlet [get-MailboxDatabase](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)Exchange Management Shell pour obtenir des informations sur les bases de données existantes. Pour plus d’informations sur l’environnement de ligne de commande Exchange Management Shell, veuillez consulter la rubrique [Exchange Server PowerShell (Environnement de ligne de commande Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
La figure suivante illustre la séquence d’événements dans une restauration classique d’une base de données Exchange gérée par le service VSS (Volume Shadow Copy Service).
  
**Figure 1. Séquence d’événements pour la restauration des bases de données**

![Diagramme présentant la séquence d’événements pour le processus de restauration. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restauration de Exchange bases de données à l’emplacement d’origine
<a name="bk_OriginalLocation"> </a>

Le rédacteur Exchange permet aux applications de restaurer les bases de données et les fichiers journaux de transactions à leurs emplacements d’origine sur Exchange serveur. Par défaut, le rédacteur Exchange relecture les fichiers journaux des transactions une fois que le demandeur a confirmé que la restauration est terminée pendant [l’opération OnPostRestore.](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) L’application de restauration doit utiliser la méthode [VSS SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) pour empêcher la relecture des fichiers journaux. Les fichiers journaux peuvent être relectés ultérieurement lorsque l’administrateur Exchange ou votre application démonte la base de données restaurée. 
  
Lors de la restauration des bases de données vers leurs objets de base de données d’origine (de telle manière que les GUID cibles dans la base de données correspondent à ceux du jeu de sauvegarde), mais à différents chemins d’accès aux fichiers, l’application doit déterminer les chemins d’accès aux fichiers actuels et restaurer les fichiers de sauvegarde dans les chemins d’accès de fichiers correspondants spécifiés dans les propriétés de base de données. Le demandeur doit appeler la méthode [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour communiquer au rédacteur Exchange l’emplacement où les fichiers sont restaurés avant que le rédacteur puisse poursuivre le processus de restauration. Si **AddNewTarget** n’est pas appelé, le rédacteur Exchange suppose que les sauvegardes sont restaurées dans les chemins d’accès aux fichiers spécifiés dans le document de métadonnées de sauvegarde. 
  
En règle générale, votre application n’a pas besoin de spécifier un nouveau chemin d’accès pour les sauvegardes effectuées à partir d’une copie du groupe de disponibilité de base de données (DAG). Exchange ne modifient généralement pas les chemins de base de données ou de fichiers journaux. Toutefois, dans une configuration DAG, l’application de sauvegarde peut avoir à spécifier les chemins de base de données et de journaux actifs, car les chemins de copie du DAG sont toujours différents de ces chemins d’accès.
  
Notez que Exchange 2013 ne prend pas en charge la restauration de copies de base de données DAG inactives. Les copies du DAG peuvent être restaurées à partir de données de sauvegarde uniquement lorsque la copie de base de données active est restaurée. L’utilisation de différents jeux de données de sauvegarde ou la tentative de restauration d’un sous-ensemble des copies de base de données peut entraîner l’in démontage de la base de données. Dans ce cas, les applications de sauvegarde n’ont pas besoin d’appeler la fonction [SetRestoreOptions,](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) car les sauvegardes sont restaurées dans les objets de base de données d’origine à partir des objets à partir de quoi elles ont été créées. Toutefois, si l’application de sauvegarde appelle **SetRestoreOptions** et que le document de métadonnées XML possède les paramètres corrects, le résultat n’est pas une erreur. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restauration de Exchange bases de données de récupération vers une base de données de récupération
<a name="bk_RecoveryDatabase"> </a>

Le rédacteur Exchange vous permet de restaurer des données directement dans une base de données de récupération. Le montage des données récupérées en tant que base de données de récupération permet à l’administrateur Exchange de restaurer des boîtes aux lettres individuelles, et même des éléments individuels dans une boîte aux lettres.
  
Si une base de données de récupération existe déjà, votre application peut démonter la base de données, restaurer les données sur la base de données de récupération et les fichiers journaux, puis la démonter.
  
Chaque Exchange 2013 ne permet de monter qu’une seule base de données de récupération à la fois. Le serveur peut contenir autant de bases de données récupérées que l’espace disque le permet, mais une seule peut être montée comme base de données de récupération. La base de données montée en tant que base de données de récupération est comptabilisée dans le nombre maximal de bases de données qui peuvent être montées à la fois. Une base de données récupérée montée en tant que base de données de récupération d’un serveur n’est associée à la boîte aux lettres d’origine d’aucune manière.
  
Pour récupérer dans une base de données de récupération, votre application doit appeler la méthode [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) et fournir un document XML qui indique les GUID de base de données source et cible. Les GUID sources doivent correspondre à ceux du jeu de sauvegarde, et les GUID cibles doivent correspondre aux entrées de base de données de destination dans AD DS. L’application de sauvegarde doit également appeler la [méthode AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier le chemin d’accès au répertoire dans lequel les fichiers sont restaurés. Si les fichiers de base de données doivent être renommés, le rédacteur Exchange renomme la base de données pendant [l’opération OnPostRestore.](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) Exchange les fichiers journaux des transactions doivent être restaurés dans un sous-dossier ( **_restoredLogs**) sous le chemin d’accès actuel du fichier journal des transactions. Si les fichiers journaux sont restaurés à un autre emplacement, le rédacteur Exchange renvoyer une erreur. Étant donné que les bases de données montées en tant que base de données de récupération ne sont pas restaurées à leur emplacement d’origine, elles doivent être mise en état d’arrêt propre avant de pouvoir être montées. Par défaut, le rédacteur Exchange place toutes les bases de données restaurées dans un état d’arrêt propre pendant la post-restauration. Si votre application de sauvegarde appelle la méthode [SetAdditionalRestores,](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) l’enregistreur Exchange ne relira pas les fichiers journaux, et l’administrateur ou votre application de sauvegarde doit mettre la base de données dans un état d’arrêt propre avant de monter la base de données. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restauration de Exchange bases de données sur un serveur de récupération
<a name="bk_RecoveryServer"> </a>

Dans certains scénarios, vous devrez peut-être récupérer un jeu de sauvegarde sur un autre serveur . Par exemple, vous devrez peut-être récupérer après une défaillance de serveur catastrophique en portant la base de données de boîtes aux lettres vers un autre serveur Exchange 2013 dans la même organisation Exchange, ou restaurer sur un serveur dédié en dehors de l’environnement de production pour récupérer les données de boîte aux lettres et de dossiers publics. 
  
Dans ces scénarios, les chemins d’accès à la base de données cible et à ses GUID d’objet sont différents de ceux de la base de données d’origine. Par conséquent, votre application doit appeler la méthode [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) avec un document XML qui indique les informations de la base de données source et cible, et appeler la méthode [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier les chemins d’accès du répertoire dans qui restaurer les fichiers de sauvegarde. Pour le rédacteur Exchange, cette restauration est identique à la restauration d’une base de données de récupération. Pour plus d’informations, [voir Restoring Exchange databases to a recovery database](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) earlier in this article. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Types d’opérations de sauvegarde Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
    

