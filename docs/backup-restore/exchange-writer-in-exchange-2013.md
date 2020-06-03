---
title: Enregistreur Exchange dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Trouvez des informations sur le rédacteur Exchange dans Exchange 2013 pour les opérations de sauvegarde et de restauration.
ms.openlocfilehash: 44270a87c38b08d274d389fa6e46f3864da13ed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452887"
---
# <a name="exchange-writer-in-exchange-2013"></a>Enregistreur Exchange dans Exchange 2013

Trouvez des informations sur le rédacteur Exchange dans Exchange 2013 pour les opérations de sauvegarde et de restauration. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange est responsable de la sauvegarde et de la restauration des bases de données Exchange Server 2013 actives. L’enregistreur Exchange prend également en charge la fonctionnalité de sauvegarde pour une base de données sélectionnée où le cliché instantané est pris par rapport à l’instance répliquée de la base de données et des fichiers journaux des transactions. 
  
## <a name="overview-of-the-exchange-writer"></a>Vue d’ensemble du rédacteur Exchange
<a name="bk_Overview"> </a>

Exchange 2013 inclut des fonctionnalités de mobilité de base de données, qui permettent de répliquer les bases de données entre différents serveurs Exchange afin d’améliorer la disponibilité de la base de données et la résilience de site. Les autres copies de base de données dans un groupe de disponibilité de base de données (DAG) fournissent une opportunité intéressante pour les sauvegardes Exchange afin d’utiliser les ressources supplémentaires disponibles dans l’emplacement de la copie. En outre, étant donné que la copie au lieu du maître de base de données actif est sauvegardée, la copie peut être indisponible pendant une période plus longue. 
  
Le rédacteur Exchange coordonne avec les services Exchange (fonctionnant pour le compte du demandeur) pour préparer les fichiers de base de données pour les sauvegardes, geler l’activité e/s résultant des transactions Exchange avant de sauvegarder la base de données, puis libérez et tronquez les fichiers journaux une fois la sauvegarde terminée.
  
Pendant une restauration, votre application de sauvegarde et de restauration demande à l’enregistreur Exchange de se coordonner avec la Banque d’identité Exchange (opérant au nom du demandeur) pour vérifier les cibles de restauration, renommer le fichier de base de données si nécessaire, puis relire les journaux de transactions en fonction des besoins. L’enregistreur Exchange prend en charge à la fois les sauvegardes et les restaurations.
  
L’enregistreur Exchange est disponible sur tous les serveurs Exchange sur lesquels le rôle serveur de boîtes aux lettres est installé. 
  
## <a name="exchange-writer-configuration-settings"></a>Paramètres de configuration du rédacteur Exchange
<a name="bk_ExchangeWriterConfig"> </a>

L’enregistreur Exchange pour VSS utilise un grand nombre de paramètres et de valeurs qui doivent être correctement définis et conservés pendant les opérations de sauvegarde et de restauration. Ces paramètres de configuration sont stockés dans le document de métadonnées de l’enregistreur Exchange. Si votre application de sauvegarde ne conserve pas ces paramètres, il se peut que vous rencontriez des erreurs inattendues lors de la tentative de sauvegarde de vos bases de données Exchange. 
  
Le tableau suivant répertorie les interfaces VSS qui exposent les métadonnées sur les composants de votre sauvegarde de base de données. Ces interfaces sont requises pour obtenir le document de métadonnées d’écriture Exchange qui est utilisé pour effectuer une sauvegarde de la Banque d’Exchange.
  
**Tableau 1. Interfaces VSS**

|**Interface VSS**|**Description**|
|:-----|:-----|
|IVssWMComponent  <br/> |Autorise l’accès aux informations de composants stockées dans l’enregistreur Exchange.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permet à l’application de demande de sauvegarde et de restauration d’examiner les métadonnées de l’enregistreur Exchange. Le document de métadonnées d’enregistreur Exchange contient les valeurs et les paramètres propres à Exchange 2013 que l’application de sauvegarde et de restauration qui demande doit pouvoir spécifier correctement les composants appropriés pour la sauvegarde.  <br/> |
|IVssComponent  <br/> |Contient les méthodes permettant d’examiner et de modifier des informations sur les composants contenus dans le document des composants de sauvegarde d’un demandeur. Les objets ne peuvent être obtenus que pour les composants qui ont été explicitement ajoutés à ce document par la méthode [IVssBackupComponents :: AddComponent](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx) .  <br/> |
|IVssBackupComponents  <br/> |Utilisé par l’application de sauvegarde et de restauration pour interroger l’enregistreur Exchange sur l’état des fichiers et exécuter les opérations de sauvegarde et de restauration. La méthode [IVssBackupComponents :: SetBackupState](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx) définit si l’opération de sauvegarde est une sauvegarde complète, copie, incrémentielle ou différentielle. La méthode [IVssBackupComponents :: AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx) définit les sous-composants d’une base de données Exchange 2013 pouvant être sélectionnée pour une opération de restauration.  <br/> |
   
Dans le système de fichiers Windows Server, une base de données Exchange 2013 est stockée sous la forme d’un fichier de base de données unique avec l’extension *. edb. Le rédacteur Exchange expose le fichier *. edb en tant que composant de base de données, tandis que les journaux de transactions (*. log) et les fichiers de point de contrôle (*. chk) sont combinés en un seul composant, connu sous le titre du composant de journal. Pour plus d’informations sur les fichiers de base de données Exchange, consultez la rubrique [concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md).
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interactions entre le rédacteur Exchange, VSS et les demandeurs VSS
<a name="bk_interactions"> </a>

Les interactions de haut niveau entre VSS, le rédacteur Exchange et Exchange 2013 pendant les opérations de sauvegarde sont les suivantes :
  
1. Le programme (ou l'agent) de sauvegarde exécute une tâche planifiée. 
    
2. Le demandeur VSS dans l’application de sauvegarde et de restauration envoie une commande au service VSS pour prendre un cliché instantané des bases de données Exchange 2013 sélectionnées. 
    
3. VSS communique avec le rédacteur Exchange pour préparer une sauvegarde de capture instantanée. Exchange 2013 interdit les actions administratives sur les bases de données, vérifie les dépendances de volume et interrompt toutes les opérations d’écriture sur l’instance sélectionnée de la base de données et des fichiers journaux de transactions tout en autorisant l’accès en lecture seule. 
    
4. VSS communique avec le fournisseur de stockage approprié pour créer un cliché instantané du volume de stockage qui contient les bases de données Exchange 2013. 
    
5. VSS publie Exchange 2013 pour reprendre les opérations ordinaires. 
    
6. Le demandeur VSS vérifie la cohérence physique du jeu de sauvegarde avant de signaler que la sauvegarde a réussi. Exchange 2013 tronque les journaux de transactions (si la base de données fait partie d’un DAG, la troncation de journal est répliquée dans toutes les copies) et enregistre l’heure de la dernière sauvegarde de la base de données.
    
VSS sérialise les interactions des demandeurs avec le rédacteur Exchange en commençant par la méthode [OnPrepareBackup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx) et en terminant par la méthode [OnPostSnapshot](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx) . En règle générale, la majorité du temps que le rédacteur Exchange passe à travailler avec le cliché instantané se produit après la méthode **OnPostSnapshot** , lorsque la cohérence du cliché instantané est vérifiée avant la fin des sauvegardes. L’enregistreur Exchange prend en charge les sauvegardes parallèles entre **OnPostSnapshot** et [OnBackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
Exchange 2013 n’autorise pas les sauvegardes simultanées de la même base de données. Une seule opération de sauvegarde peut être exécutée sur une base de données donnée à la fois. Lorsque la sauvegarde est en cours d’exécution, la Banque d’Exchange place la base de données dans un état de sauvegarde en cours. Cet État en mémoire est effacé au terme du processus de sauvegarde ou au redémarrage du service. L’état de sauvegarde en mémoire et les données associées sont perdus lorsque le service qui héberge l’enregistreur Exchange est redémarré, lorsque le système d’exploitation est redémarré ou lorsqu’un basculement de cluster se produit. L’un de ces événements entraîne l’échec du travail de sauvegarde.
  
La troncation du fichier journal des transactions initiées par une sauvegarde est déclenchée en fonction du type de sauvegarde à effectuer. Dans les configurations non DAG, l’enregistreur Exchange tronque les fichiers journaux des transactions à la fin des sauvegardes complètes ou incrémentielles réussies. Dans les configurations répliquées DAG, la troncation des journaux est retardée par le service de réplication jusqu’à ce que tous les fichiers journaux nécessaires soient relus dans toutes les autres copies. Le service de réplication supprime les fichiers journaux sauvegardés des chemins d’accès au fichier journal actifs et de copie une fois qu’il a vérifié que les fichiers journaux ont bien été appliqués à la base de données de copie et à la base de données active et que le point de contrôle des copies de base de données a passé les fichiers journaux à supprimer.
  
## <a name="see-also"></a>Voir aussi

- [Journaux de transaction et fichiers de point de contrôle pour la sauvegarde et la restauration dans Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

