---
title: Enregistreur Exchange dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Trouvez des informations sur l’auteur du message Exchange dans Exchange 2013 pour la sauvegarde et de restauration des opérations.
ms.openlocfilehash: a4dc5963ab24a83969efc6e425b38a35276f3aa3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754742"
---
# <a name="exchange-writer-in-exchange-2013"></a>Enregistreur Exchange dans Exchange 2013

Trouvez des informations sur l’auteur du message Exchange dans Exchange 2013 pour la sauvegarde et de restauration des opérations. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange est chargé de la sauvegarde et la restauration de bases de données actives Exchange Server 2013. Le rédacteur Exchange prend également en charge la fonctionnalité de sauvegarde pour une base de données sélectionné où le cliché par rapport à l’instance de la base de données et des transactions répliquée fichiers journaux. 
  
## <a name="overview-of-the-exchange-writer"></a>Vue d’ensemble de l’enregistreur Exchange
<a name="bk_Overview"> </a>

Exchange 2013 inclut des fonctionnalités de mobilité de base de données, qui permettent de bases de données doivent être répliquées entre les différents serveurs Exchange pour améliorer la disponibilité de base de données et la résilience de site. Les autres copies de base de données dans un groupe de disponibilité de base de données (DAG) offrent une opportunité précieuse pour les sauvegardes Exchange à utiliser les ressources supplémentaires qui sont disponibles à l’emplacement de copie. En outre, étant donné que la copie au lieu de la base de données active master est sauvegardée, la copie peut être indisponible pendant la sauvegarde pour une période plus longue. 
  
Le rédacteur Exchange coordonnées avec les services Exchange (en fonctionnement au nom du demandeur) pour préparer les fichiers de base de données pour les sauvegardes, Figer l’activité d’e/s résultant de Exchange transactions avant la sauvegarde de la base de données, puis libérer et tronquer les fichiers journaux une fois la sauvegarde terminée.
  
Lors d’une restauration, votre application de sauvegarde et de restauration indique à l’auteur du message change pour coordonner avec la banque d’informations Exchange (en fonctionnement au nom du demandeur) pour vérifier les cibles de restauration, renommez le fichier de base de données si nécessaire, puis réexécuter la transaction journaux selon vos besoins. Le rédacteur Exchange prend en charge les sauvegardes et restaurations.
  
Le rédacteur Exchange est disponible sur tout serveur Exchange qui a le rôle serveur de boîtes aux lettres. 
  
## <a name="exchange-writer-configuration-settings"></a>Paramètres de configuration Exchange writer
<a name="bk_ExchangeWriterConfig"> </a>

Le rédacteur Exchange pour VSS utilise une variété de paramètres et les valeurs qui doivent être correctement et conservés pendant les opérations de sauvegarde et de restauration. Ces paramètres de configuration sont stockés dans le document de métadonnées du rédacteur Exchange. Si votre application de sauvegarde ne conserve pas ces paramètres, vous pouvez rencontrer des erreurs inattendues lorsque vous essayez de sauvegarder vos bases de données Exchange. 
  
Le tableau suivant répertorie les interfaces VSS qui exposent des métadonnées sur les composants de sauvegarde de votre base de données. Ces interfaces sont nécessaires pour obtenir l’enregistreur Exchange document de métadonnées qui sert à effectuer une sauvegarde de la banque d’informations Exchange.
  
**Le tableau 1. Interfaces VSS**

|**Interface VSS**|**Description**|
|:-----|:-----|
|IVssWMComponent  <br/> |Permet d’accéder aux informations sur le composant stockées dans l’enregistreur Exchange.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permet à l’application de sauvegarde et restauration de la demande examiner les métadonnées du rédacteur Exchange. Le document de métadonnées du rédacteur Exchange contient des valeurs spécifiques de Exchange 2013 et paramètres de l’application de sauvegarde et de restauration émet requiert afin qu’il puisse spécifier correctement les composants appropriés pour la sauvegarde.  <br/> |
|IVssComponent  <br/> |Contient des méthodes pour examiner et de modifier des informations sur les composants contenus dans le Document des composants de sauvegarde d’un demandeur. Objets peuvent être obtenus uniquement pour les composants qui ont été explicitement ajoutés à ce document par la méthode [IVssBackupComponents::AddComponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382646%28v=vs.85%29.aspx) .  <br/> |
|IVssBackupComponents  <br/> |Utilisée par l’application de sauvegarde et de restauration demande d’interroger l’enregistreur Exchange sur l’état du fichier et de sauvegarde et les opérations de restauration. La méthode [IVssBackupComponents::SetBackupState](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382833%28v=vs.85%29.aspx) définit si l’opération de sauvegarde est une copie complète, incrémentielle, ou sauvegarde différentielle. La méthode [IVssBackupComponents::AddRestoreSubcomponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382649%28v=vs.85%29.aspx) définit les sous-composants d’une base de données Exchange 2013 qui peut être sélectionné pour une opération de restauration.  <br/> |
   
Dans le système de fichiers Windows Server, une base de données Exchange 2013 est enregistrée comme un fichier de base de données unique avec une extension *.edb. Expose l’enregistreur Exchange le *.edb que le composant de base de données, tout en les journaux de transactions (*.log) et les fichiers de point de contrôle (*.chk) sont regroupés dans un seul composant, désigné en tant que composant du journal. Pour plus d’informations sur les fichiers de base de données Exchange, consultez la rubrique [concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md).
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interactions entre l’enregistreur Exchange, VSS et VSS demandeurs
<a name="bk_interactions"> </a>

L’interaction de haut niveau entre le service VSS, le rédacteur Exchange, et Exchange 2013 pendant les opérations de sauvegarde est comme suit :
  
1. Le programme de sauvegarde (ou agent) exécute une tâche planifiée. 
    
2. Le demandeur VSS dans l’application de sauvegarde et restauration envoie une commande au service VSS visant à prendre un cliché instantané des bases de données Exchange 2013 sélectionnés. 
    
3. Service VSS communique avec l’enregistreur Exchange pour préparer une sauvegarde instantanée. Exchange 2013 interdit les actions d’administration sur les bases de données, vérifie les dépendances du volume et suspend toutes les opérations d’écriture pour l’instance sélectionnée des base de données et les fichiers journaux tout en autorisant l’accès en lecture seule. 
    
4. Service VSS communique avec le fournisseur de stockage approprié pour créer un cliché instantané du volume de stockage qui contient les bases de données Exchange 2013. 
    
5. VSS libère Exchange 2013 pour les opérations ordinaires. 
    
6. Le demandeur VSS vérifie la cohérence de la sauvegarde avant que la sauvegarde a réussi de signalisation physique. Exchange 2013 tronque les journaux de transactions (si la base de données fait partie d’un DAG, la troncation de journal est répliquée sur toutes les copies) et enregistre l’heure de la dernière sauvegarde pour la base de données.
    
VSS sérialiser l’interaction des demandeurs avec l’enregistreur Exchange commençant par la méthode [OnPrepareBackup](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381571%28v=vs.85%29.aspx) et se terminant par la méthode [OnPostSnapshot](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381568%28v=vs.85%29.aspx) . En règle générale, la majorité du temps de l’enregistreur Exchange travailler avec le cliché instantané se produit après la méthode **OnPostSnapshot** , une fois que la cohérence du cliché instantané est vérifiée avant l’achèvement des sauvegardes. Le rédacteur Exchange prend en charge les sauvegardes en parallèle entre **OnPostSnapshot** et [OnBackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
Exchange 2013 n’autorise pas les sauvegardes simultanées de la même base de données. Qu’une seule opération de sauvegarde peut exécutée sur une base de données en même temps. Lorsque la sauvegarde est en cours d’exécution, la banque d’informations Exchange place la base de données dans un état de la sauvegarde en cours. Cet état en mémoire est désactivé soit à la fin du processus de sauvegarde ou lorsque le service est redémarré. L’état de la sauvegarde en cours en mémoire et les données associées sont perdues lorsque le service qui héberge l’enregistreur Exchange est redémarré lors du redémarrage du système d’exploitation, ou un cluster de basculement se produit. Une de ces événements entraîne la sauvegarde échoue.
  
Sauvegarde lancée fichier troncature de journal est déclenchée en fonction du type de sauvegarde à effectuer. Dans les configurations non DAG, le rédacteur Exchange tronque les fichiers journaux de transactions à l’issue de sauvegardes complètes ou incrémentielles réussies. Dans DAG répliqués configurations, la troncation de journal sera retardée par le service de réplication jusqu'à ce que tous les fichiers journaux nécessaires ont été relus dans toutes les autres copies. Le service de réplication supprimera sauvegardé les fichiers journaux à la fois actif et la copie de chemins des fichiers journaux une fois qu’il vérifie que les fichiers journaux ont bien été appliqués à la base de données de copie et deux bases de données active et le point de contrôle de copies de base de données a réussi. les fichiers journaux à supprimer.
  
## <a name="see-also"></a>Voir aussi

- [Les journaux de transactions et des fichiers de point de contrôle pour la sauvegarde et de restauration dans Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

