---
title: Restauration des bases de données Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Trouvez des informations sur les différentes méthodes de restauration de vos bases de données Exchange 2013.
ms.openlocfilehash: 9fe417bda5dc728af619da02d62ada6e920f731d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528672"
---
# <a name="restoring-exchange-2013-databases"></a>Restauration des bases de données Exchange 2013

Trouvez des informations sur les différentes méthodes de restauration de vos bases de données Exchange 2013. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange qui est inclus dans Exchange Server 2013 offre une flexibilité suffisante pour la restauration de vos bases de données Exchange. À l’aide de l’enregistreur Exchange dans Exchange 2013, vous pouvez restaurer vos sauvegardes de clichés instantanés aux emplacements suivants :
  
- La base de données d’origine, que la configuration de la base de données ou du fichier journal des transactions ait été modifiée.
    
- Une base de données de récupération.
    
- Toute base de données de production, que le nom complet de la base de données corresponde ou non au nom d’un jeu de sauvegarde VSS.
    
Lorsque votre application de restauration restaure les informations dans la base de données d’origine, les fichiers journaux doivent être restaurés dans le chemin d’accès du répertoire spécifié dans les services de domaine Active Directory (AD DS) pour cette base de données. Si votre application restaure une base de données à un autre emplacement, les fichiers journaux doivent être restaurés dans un dossier nommé **_restoredLogs** qui se trouve dans le répertoire du fichier journal de la base de données. 
  
Lors de la restauration vers un serveur ou une base de données qui est différente de la base de données d’origine, votre application de restauration doit s’assurer que les chemins d’accès aux répertoires de base de données fournis à VSS correspondent à ceux dans AD DS. Vous pouvez utiliser la cmdlet [Get-MailboxDatabase](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)Exchange Management Shell pour obtenir des informations sur les bases de données existantes. Pour plus d’informations sur l’environnement de commande Exchange Management Shell, consultez la rubrique [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
La figure suivante illustre la séquence d’événements dans une restauration standard d’une base de données Exchange gérée par le service VSS (Volume Shadow Copy Service).
  
**Figure 1. Séquence des événements de restauration des bases de données**

![Diagramme présentant la séquence d’événements pour le processus de restauration. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restauration des bases de données Exchange à l’emplacement d’origine
<a name="bk_OriginalLocation"> </a>

L’enregistreur Exchange permet aux applications de restaurer les bases de données et les fichiers journaux des transactions à leurs emplacements d’origine sur le serveur Exchange. Par défaut, le rédacteur Exchange relit les fichiers journaux des transactions une fois que le demandeur confirme que la restauration est terminée pendant l’opération [OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . L’application de restauration doit utiliser la méthode VSS [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) pour empêcher la relecture des fichiers journaux. Les fichiers journaux peuvent être relus ultérieurement lorsque l’administrateur Exchange ou votre application remonte la base de données restaurée. 
  
Lorsque vous restaurez des bases de données vers leurs objets de base de données d’origine (par exemple, les GUID cibles de la base de données correspondent à ceux du jeu de sauvegarde) mais aux chemins d’accès aux fichiers, l’application doit déterminer les chemins d’accès aux fichiers actuels et restaurer les fichiers de sauvegarde dans les chemins de fichiers correspondants spécifiés dans les propriétés de la base de données. Le demandeur doit appeler la méthode [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour communiquer avec le rédacteur Exchange l’emplacement où les fichiers sont restaurés avant que le rédacteur puisse poursuivre le processus de restauration. Si **AddNewTarget** n’est pas appelé, le writer Exchange suppose que les sauvegardes soient restaurées dans les chemins d’accès aux fichiers spécifiés dans le document de métadonnées de sauvegarde. 
  
En règle générale, votre application n’a pas besoin de spécifier un nouveau chemin d’accès pour les sauvegardes effectuées à partir d’une copie de groupe de disponibilité de base de données (DAG). Les administrateurs Exchange ne modifient généralement pas les chemins d’accès aux fichiers journaux ou de base de données. Dans une configuration DAG, toutefois, l’application de sauvegarde peut être amenée à spécifier les chemins d’accès de base de données et de journal actifs, car les chemins de copie de DAG sont toujours différents de ces chemins d’accès.
  
Notez qu’Exchange 2013 ne prend pas en charge la restauration des copies de base de données DAG inactives. Les copies DAG peuvent être restaurées à partir de données de sauvegarde uniquement lorsque la copie de base de données active est restaurée. L’utilisation de différents jeux de données de sauvegarde ou la tentative de restauration d’un sous-ensemble des copies de base de données peut entraîner le démontage de la base de données. Les applications de sauvegarde n’ont pas besoin d’appeler la fonction [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) dans ce cas, car les sauvegardes sont restaurées dans les objets de base de données d’origine à partir desquels ils ont été créés. Toutefois, si l’application de sauvegarde appelle **SetRestoreOptions** et que le document de métadonnées XML possède les paramètres corrects, le résultat ne correspond pas à une erreur. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restauration de bases de données Exchange dans une base de données de récupération
<a name="bk_RecoveryDatabase"> </a>

Le rédacteur Exchange vous permet de restaurer des données directement dans une base de données de récupération. Le montage des données récupérées en tant que base de données de récupération permet à l’administrateur Exchange de restaurer des boîtes aux lettres individuelles et même des éléments individuels dans une boîte aux lettres.
  
Si une base de données de récupération existe déjà, votre application peut démonter la base de données, restaurer les données dans la base de données de récupération et les fichiers journaux, puis remonter la base de données.
  
Chaque serveur Exchange 2013 ne permet de monter qu’une seule base de données de récupération à la fois. Le serveur peut contenir autant de bases de données récupérées que l’espace disque le permet, mais un seul peut être monté en tant que base de données de récupération. La base de données montée en tant que base de données de récupération est comptabilisée dans le nombre maximal de bases de données qui peuvent être montées à la fois. Une base de données récupérée, montée en tant que base de données de récupération d’un serveur, n’est pas associée à la boîte aux lettres d’origine.
  
Pour récupérer une base de données de récupération, votre application doit appeler la méthode [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) et fournir un document XML qui indique les GUID de base de données source et cible. Les GUID sources doivent correspondre à ceux du jeu de sauvegarde et les GUID cibles doivent correspondre aux entrées de la base de données de destination dans AD DS. L’application de sauvegarde doit également appeler la méthode [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier le chemin d’accès au répertoire dans lequel les fichiers sont restaurés. Si les fichiers de base de données doivent être renommés, l’enregistreur Exchange renomme la base de données pendant l’opération [OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . Exchange exige que les fichiers journaux des transactions soient restaurés dans un sous-dossier ( **_restoredLogs**) sous le chemin d’accès au fichier journal des transactions actuel. Si les fichiers journaux sont restaurés à un autre emplacement, le rédacteur Exchange renvoie une erreur. Étant donné que les bases de données en cours de montage en tant que base de données de récupération ne sont pas restaurées à leur emplacement d’origine, elles doivent être mises en état d’arrêt correct avant de pouvoir être montées. Par défaut, l’enregistreur Exchange place toutes les bases de données restaurées dans un état d’arrêt correct pendant la post-restauration. Si votre application de sauvegarde appelle la méthode [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) , le rédacteur Exchange ne lit pas les fichiers journaux, et l’administrateur ou votre application de sauvegarde doit mettre la base de données en état d’arrêt correct avant de monter la base de données. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restauration de bases de données Exchange sur un serveur de récupération
<a name="bk_RecoveryServer"> </a>

Dans certains cas, vous devrez peut-être récupérer un jeu de sauvegarde sur un autre serveur ; Par exemple, vous pouvez être amené à effectuer une récupération suite à une défaillance catastrophique du serveur en transférant la base de données de boîtes aux lettres vers un autre serveur Exchange 2013 de la même organisation Exchange ou une restauration sur un serveur dédié en dehors de l’environnement de production afin de récupérer les données de boîtes aux lettres et de dossiers publics. 
  
Dans ces scénarios, les chemins d’accès aux fichiers de la base de données cible, ainsi que ses GUID d’objet, diffèrent de ceux de la base de données d’origine. Par conséquent, votre application doit appeler la méthode [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) avec un document XML qui indique les informations de la base de données source et cible, et appeler la méthode [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier les chemins d’accès de répertoire vers lesquels restaurer les fichiers de sauvegarde. Pour le rédacteur Exchange, cette restauration est identique à celle de la restauration d’une base de données de récupération. Pour plus d’informations, consultez la rubrique [restauration de bases de données Exchange sur une base de données de récupération](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) plus haut dans cet article. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Référence de classe fonction cchksgfiles](cchksgfiles-class-reference.md)
    

