---
title: Restauration des bases de données Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Trouvez des informations sur les différentes méthodes que vous pouvez restaurer vos bases de données Exchange 2013.
ms.openlocfilehash: d3ca3a884b0ad30f7d7968a9ed435b02aaf205e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754775"
---
# <a name="restoring-exchange-2013-databases"></a>Restauration des bases de données Exchange 2013

Trouvez des informations sur les différentes méthodes que vous pouvez restaurer vos bases de données Exchange 2013. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange qui est inclus dans Exchange que Server 2013 autorise une certaine souplesse dans la façon dont vous restaurez vos bases de données Exchange. À l’aide de l’enregistreur Exchange dans Exchange 2013, vous pouvez restaurer vos clichés instantanés aux emplacements suivants :
  
- La base d’origine, indépendamment de si la configuration de chemin d’accès de fichier journal de base de données ou de la transaction a été modifiée.
    
- Une base de données de récupération.
    
- Toute base de données production, quel que soit ou non le nom d’affichage de base de données correspond au nom d’un jeu de sauvegarde VSS.
    
Lorsque votre application de restauration restaure les informations pour la base de données d’origine, les fichiers journaux doivent être restaurés dans le répertoire spécifié dans les Services de domaine Active Directory (AD DS) pour cette base de données. Si votre application restaure une base de données vers un autre emplacement, les fichiers journaux doivent être restaurés à un dossier nommé **_restoredLogs** qui se trouve dans le répertoire du fichier journal de base de données. 
  
Lors de la restauration sur un serveur ou une base de données qui est différent de celui de la base de données d’origine, votre application de restauration devez vous assurer que les chemins d’accès du répertoire de base de données fournis pour VSS correspondent à celles dans AD DS. Vous pouvez utiliser l’applet de commande [get-MailboxDatabase](http://technet.microsoft.com/en-us/library/bb124924%28v=exchg.150%29.aspx)Exchange Management Shell pour obtenir des informations sur les bases de données existantes. Pour plus d’informations sur Exchange Management Shell, voir [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
La figure suivante illustre la séquence d’événements dans une restauration classique d’une base de données Exchange qui est géré par Volume Shadow Copy Service (VSS).
  
**La figure 1. Séquence d’événements pour la restauration des bases de données**

![Diagramme présentant la séquence d’événements pour le processus de restauration. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restauration des bases de données Exchange à l’emplacement d’origine
<a name="bk_OriginalLocation"> </a>

Le rédacteur Exchange permet aux applications restaurer les bases de données et fichiers journaux des transactions à leurs emplacements d’origine sur le serveur Exchange. Par défaut, le rédacteur Exchange relit les fichiers journaux des transactions une fois que le demandeur confirme que la restauration est terminée pendant l’opération [OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . L’application de restauration doit utiliser la méthode VSS [SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx) pour éviter d’avoir les fichiers journaux relus. Les fichiers journaux peuvent être relus à une date ultérieure lorsque l’administrateur Exchange ou votre application remonte la base de données restaurée. 
  
Lorsque les objets restauration des bases de données à la base de données d’origine (telles que la cible de la base de données GUID correspondent à ceux du jeu de sauvegarde) mais à différents chemins d’accès, l’application doit déterminer les chemins d’accès du fichier en cours et restaurer les fichiers de sauvegarde pour le chemins de fichier correspondants spécifiés dans les propriétés de base de données. Le demandeur doit appeler la méthode [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour communiquer avec l’auteur du message change l’emplacement où les fichiers sont restaurés que le rédacteur puisse continuer avec le reste du processus de restauration. Si **AddNewTarget** n’est pas appelée, le rédacteur Exchange suppose que les sauvegardes sont restaurés dans les chemins d’accès de fichier spécifiés dans le document de métadonnées de sauvegarde. 
  
En règle générale, votre application ne doit pas spécifier un nouveau chemin d’accès pour les sauvegardes sont effectuées à partir d’une copie du groupe de disponibilité de base de données (DAG). Les administrateurs Exchange ne modifient pas généralement les chemins d’accès de fichier de base de données ou de journal. Dans une configuration DAG, toutefois, l’application de sauvegarde peut-être spécifier la base de données active et enregistrer les chemins d’accès, car les chemins d’accès de la copie DAG seront toujours différents de ces chemins d’accès.
  
Notez que Exchange 2013 ne prend pas en charge restauration de copies de base de données inactives DAG. Copies DAG peuvent être restaurés à partir des données de sauvegarde uniquement lorsque la copie active de la base de données est restaurée. À l’aide de différents ensembles de données de sauvegarde ou essayez de restaurer un sous-ensemble des copies de base de données peut entraîner la base de données de devenir irrécupérable. Applications de sauvegarde est inutile d’appeler la fonction [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) dans ce cas, étant donné que les sauvegardes sont restaurés dans les objets de base de données d’origine, qu'ils ont été créés à partir. Toutefois, si l’application de sauvegarde appelle **SetRestoreOptions** et le document de métadonnées XML avec les paramètres corrects, le résultat n’est pas une erreur. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restauration des bases de données Exchange vers une base de données de récupération
<a name="bk_RecoveryDatabase"> </a>

Le rédacteur Exchange permet de restaurer les données directement dans une base de données de récupération. Les données récupérées comme une base de données de récupération de montage permet à l’administrateur Exchange restaurer des boîtes aux lettres et des éléments de même individuels dans une boîte aux lettres.
  
Si une base de données de récupération existe déjà, votre application peut démonter la base de données, restaurez les données sur les récupération de base de données et les fichiers journaux et remontez la base de données.
  
Chaque serveur Exchange 2013 ne permet qu’une seule base de données de récupération doit être monté à la fois. Le serveur peut contenir autant bases de données restaurées comme permet d’espace disque, mais peut uniquement être monté en tant que la base de données de récupération. La base de données montée la base de données de récupération est comptabilisé dans le nombre maximal de bases de données qui peut être monté à la fois. Une base de données récupérée montée comme base de données de récupération d’un serveur n’est pas associé à la boîte aux lettres d’origine en aucune façon.
  
Pour restaurer une base de données de récupération, votre application doit appeler la méthode [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) et fournir un document XML qui indique la source et cible le GUID de la base de données. La GUID de la source doit correspondre à ceux du jeu de sauvegarde, et la GUID de la cible doit correspondre les entrées de base de données de destination dans AD DS. L’application de sauvegarde doit également appeler la méthode [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier le chemin d’accès du répertoire dans lequel les fichiers sont restaurés. Si les fichiers de base de données doivent être renommés, le rédacteur Exchange renomme la base de données pendant l’opération [OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . Exchange requiert les fichiers journaux des transactions à restaurer dans un sous-dossier ( **_restoredLogs**) sous le chemin du fichier journal des transactions en cours. Si les fichiers journaux sont restaurés à tout autre emplacement, le rédacteur Exchange renvoie une erreur. Être montés en tant que la base de données de récupération des bases de données ne sont pas restaurés à leur emplacement d’origine, il est nécessaire de mettre en état d’arrêt correct avant d’être montés. Par défaut, le rédacteur Exchange s’affiche toutes les bases de données restaurées dans un état d’arrêt correct pendant post-restauration. Si votre application de sauvegarde appelle la méthode [SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx) , le rédacteur Exchange ne sera pas relire les fichiers journaux et l’administrateur ou votre application de sauvegarde doit mettre la base de données dans un état d’arrêt correct avant de montage le base de données. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restauration des bases de données Exchange sur un serveur de récupération
<a name="bk_RecoveryServer"> </a>

Dans certains scénarios, vous devrez peut-être récupérer une jeu de sauvegarde vers un autre serveur ; Par exemple, vous devrez peut-être récupérer à partir d’un échec majeur sur le serveur par le transfert de la base de données de boîtes aux lettres vers un autre serveur Exchange 2013 dans la même organisation Exchange, ou de restauration sur un serveur dédié à l’extérieur de l’environnement de production pour récupérer les boîtes aux lettres et données de dossiers publics. 
  
Dans ces scénarios, les chemins d’accès de fichier pour la base de données cible, ainsi que son GUID d’objet sont différentes de celles de la base de données d’origine. Par conséquent, votre application doit appeler la méthode [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) avec un document XML qui indique la source et informations de base de données cible et appelez la méthode [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) pour spécifier les chemins d’accès pour restaurer les fichiers de sauvegarde . Pour l’auteur du message change, cette restauration est identique à la restauration d’une base de données de récupération. Pour plus d’informations, voir [Exchange de restauration des bases de données à une base de données de récupération](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) plus haut dans cet article. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Créer la sauvegarde et de restaurer des applications pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
    

