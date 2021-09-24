---
title: Exchange rédacteur en Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Trouvez des informations sur le rédacteur Exchange dans Exchange 2013 pour les opérations de sauvegarde et de restauration.
ms.openlocfilehash: 7c50c2aa014308b05bdbc1acf0f2a91e33717ed6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516236"
---
# <a name="exchange-writer-in-exchange-2013"></a>Exchange rédacteur en Exchange 2013

Trouvez des informations sur le rédacteur Exchange dans Exchange 2013 pour les opérations de sauvegarde et de restauration. 
  
**S’applique à :** Exchange Server 2013 
  
Le rédacteur Exchange est responsable de la sauvegarde et de la restauration des bases de données actives Exchange Server 2013. Le rédacteur Exchange prend également en charge la fonctionnalité de sauvegarde pour une base de données sélectionnée dans laquelle le shadow copy est pris en compte par rapport à l’instance répliquée de la base de données et des fichiers journaux de transactions. 
  
## <a name="overview-of-the-exchange-writer"></a>Vue d’ensemble du rédacteur Exchange’équipe
<a name="bk_Overview"> </a>

Exchange 2013 inclut des fonctionnalités de mobilité de base de données, qui permettent de répliquer des bases de données entre différents serveurs Exchange afin d’améliorer la disponibilité des bases de données et la résilience de site. Les autres copies de base de données dans un groupe de disponibilité de base de données (DAG) offrent une opportunité précieuse aux sauvegardes Exchange d’utiliser les ressources supplémentaires disponibles sur l’emplacement de copie. En outre, étant donné que la copie au lieu de la base de données maître active est sauvegarde, la copie peut être indisponible pendant la sauvegarde pendant une période plus longue. 
  
L’enregistreur Exchange se coordonne avec les services Exchange (fonctionnant au nom du demandeur) pour préparer les fichiers de base de données pour les sauvegardes, figer l’activité d’E/S résultant des transactions Exchange avant de sauvegarder la base de données, puis libérer et tronqué les fichiers journaux une fois la sauvegarde terminée.
  
Pendant une restauration, votre application de sauvegarde et de restauration demande à l’enregistreur Exchange de se coordonner avec le magasin Exchange (fonctionnant pour le compte du demandeur) pour vérifier les cibles de restauration, renommer le fichier de base de données si nécessaire, puis relire les journaux des transactions si nécessaire. Le rédacteur Exchange prend en charge les sauvegardes et les restaurations.
  
Le rédacteur Exchange est disponible sur n’importe quel serveur Exchange sur qui le rôle serveur de boîtes aux lettres est installé. 
  
## <a name="exchange-writer-configuration-settings"></a>Exchange de configuration de l’auteur de l’écriture
<a name="bk_ExchangeWriterConfig"> </a>

Le rédacteur Exchange vsS utilise une variété de paramètres et de valeurs qui doivent être correctement définies et conservées pendant les opérations de sauvegarde et de restauration. Ces paramètres de configuration sont stockés dans le document de métadonnées Exchange rédacteur. Si votre application de sauvegarde ne conserve pas ces paramètres, vous risquez de faire face à des erreurs inattendues lorsque vous tentez de sauvegarder vos bases de données Exchange données. 
  
Le tableau suivant répertorie les interfaces VSS qui exposent les métadonnées sur les composants de votre sauvegarde de base de données. Ces interfaces sont requises pour obtenir le document de métadonnées Exchange rédacteur utilisé pour effectuer une sauvegarde du magasin Exchange de données.
  
**Tableau 1. Interfaces VSS**

|**Interface VSS**|**Description**|
|:-----|:-----|
|IVssWMComponent  <br/> |Permet d’accéder aux informations de composant stockées dans l’Exchange rédacteur.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permet à l’application de sauvegarde et de restauration de demande d’examiner les métadonnées du rédacteur Exchange de données. Le document de métadonnées du rédacteur Exchange contient des valeurs et des paramètres spécifiques à Exchange 2013 dont l’application de sauvegarde et de restauration demande, afin qu’elle puisse spécifier correctement les composants appropriés pour la sauvegarde.  <br/> |
|IVssComponent  <br/> |Contient des méthodes pour examiner et modifier des informations sur les composants contenus dans le document des composants de sauvegarde d’un demandeur. Les objets peuvent uniquement être obtenus pour les composants qui ont été explicitement ajoutés à ce document par la méthode [IVssBackupComponents::AddComponent.](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx)  <br/> |
|IVssBackupComponents  <br/> |Utilisé par l’application de sauvegarde et de restauration pour demander au rédacteur Exchange l’état du fichier et pour exécuter des opérations de sauvegarde et de restauration. La [méthode IVssBackupComponents::SetBackupState ](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx) définit si l’opération de sauvegarde est une sauvegarde complète, copie, incrémentielle ou différentielle. La méthode [IVssBackupComponents::AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx) définit les sous-ensembles d’une base de données Exchange 2013 qui peuvent être sélectionnés pour une opération de restauration.  <br/> |
   
Dans le système de fichiers Windows Server, une base de données Exchange 2013 est stockée en tant que fichier de base de données unique avec une extension *.edb. Le rédacteur Exchange expose *le fichier .edb** en tant que composant de base de données, tandis que les journaux des transactions ( .log) et les fichiers de point de contrôle ( .chk) sont combinés en un seul composant, appelé composant journal. Pour plus d’informations Exchange fichiers de base de données, voir les concepts de sauvegarde et [de restauration Exchange 2013.](backup-and-restore-concepts-for-exchange-2013.md)
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interactions entre le rédacteur Exchange, VSS et les demandeurs VSS
<a name="bk_interactions"> </a>

L’interaction de haut niveau entre le service VSS, le rédacteur Exchange et Exchange 2013 lors des opérations de sauvegarde est la suivante :
  
1. Le programme (ou l'agent) de sauvegarde exécute une tâche planifiée. 
    
2. Le demandeur VSS dans l’application de sauvegarde et de restauration envoie une commande au système VSS pour prendre un shadow copy des bases de données Exchange 2013 sélectionnées. 
    
3. VSS communique avec le rédacteur Exchange pour préparer une sauvegarde de capture instantanée. Exchange 2013 interdit les actions administratives sur les bases de données, vérifie les dépendances de volume et suspend toutes les opérations d’écriture sur l’instance sélectionnée de la base de données et des fichiers journaux des transactions tout en permettant un accès en lecture seule. 
    
4. VSS communique avec le fournisseur de stockage approprié pour créer un shadow copy du volume de stockage qui contient les bases de données Exchange 2013. 
    
5. VSS publie Exchange 2013 pour reprendre les opérations ordinaires. 
    
6. Le demandeur VSS vérifie la cohérence physique du jeu de sauvegarde avant de signaler que la sauvegarde a réussi. Exchange 2013 tronque les journaux de transactions (si la base de données fait partie d’un DAG, la troncation des journaux est répliquée parmi toutes les copies) et enregistre l’heure de la dernière sauvegarde de la base de données.
    
VSS sérialise l’interaction des demandeurs avec le rédacteur Exchange en commençant par la méthode [OnPrepareBackup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx) et en terminant par la méthode [OnPostSnapshot.](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx) En règle générale, la majorité du temps passé par le rédacteur Exchange à travailler sur le shadow copy se produit après la méthode **OnPostSnapshot,** lorsque la cohérence du shadow copy est vérifiée avant la fin des sauvegardes. Le rédacteur Exchange prend en charge les sauvegardes parallèles entre **OnPostSnapshot** et [OnBackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
Exchange 2013 n’autorise pas les sauvegardes simultanées de la même base de données. Un seul travail de sauvegarde peut s’exécuter sur une base de données donnée à la fois. Lorsque la sauvegarde est en cours d’exécution, le magasin Exchange place la base de données dans un état de sauvegarde en cours. Cet état en mémoire est effacé à la fin du processus de sauvegarde ou au redémarrage du service. L’état de sauvegarde en cours en mémoire et les données associées sont perdus lorsque le service qui héberge le rédacteur Exchange est redémarré, lorsque le système d’exploitation est redémarré ou lorsqu’un cluster se produit. L’un de ces événements entraîne l’échec du travail de sauvegarde.
  
La troncation du fichier journal des transactions initiée par la sauvegarde est déclenchée en fonction du type de sauvegarde à effectuer. Dans les configurations autres que DAG, le rédacteur Exchange tronqué les fichiers journaux des transactions à la fin des sauvegardes complètes ou incrémentielles réussies. Dans les configurations répliquées par DAG, la troncation des journaux est retardée par le service de réplication jusqu’à ce que tous les fichiers journaux nécessaires soient relectés dans toutes les autres copies. Le service de réplication supprime les fichiers journaux à la fois des chemins d’accès actifs et des fichiers journaux de copie après avoir vérifié que les fichiers journaux ont été correctement appliqués à la base de données de copie et que la base de données active et le point de contrôle des copies de base de données ont passé les fichiers journaux à supprimer.
  
## <a name="see-also"></a>Voir aussi

- [Journaux des transactions et fichiers de point de contrôle pour la sauvegarde et la restauration Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

