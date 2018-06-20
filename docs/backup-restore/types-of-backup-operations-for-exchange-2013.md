---
title: Types d’opérations de sauvegarde pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Trouvez des informations sur les différents types de sauvegardes que vous pouvez effectuer sur votre Exchange 2013 stocker les bases de données, y compris complète, copie, incrémentielle et les sauvegardes différentielles.
ms.openlocfilehash: 588bc0ffe896f286258006f7f123cf09d28b218c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754790"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Types d’opérations de sauvegarde pour Exchange 2013

Trouvez des informations sur les différents types de sauvegardes que vous pouvez effectuer sur votre Exchange 2013 stocker les bases de données, y compris complète, copie, incrémentielle et les sauvegardes différentielles.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les différents types de sauvegardes que vous pouvez effectuer sur les bases de données Exchange Server 2013, et comment ces sauvegardes affectent les fichiers de base de données. 
  
Sauvegarde et restauration des applications qui utilisent le Volume Shadow Copy Service (VSS) et l’auteur du message Exchange peuvent effectuer les types de sauvegardes répertoriées dans le tableau suivant.
  
**Le tableau 1. Types d’opérations de sauvegarde**

|**Type de sauvegarde**|**Description**|
|:-----|:-----|
|[Sauvegardes complètes](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Sauvegarde les bases de données (\*.edb), les journaux de transactions (\*.log), les fichiers de point de contrôle (\*.chk) et puis tronque les journaux des transactions pour une base de données spécifique.  <br/> |
|[Copier les sauvegardes](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Sauvegarde la base de données, les journaux de transactions et les fichiers de point de contrôle. Les sauvegardes ne tronquent les journaux des transactions pour la base de données.  <br/> |
|[Sauvegardes incrémentielles](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Sauvegarde des journaux des transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle, puis tronque les journaux de transactions.  <br/> |
|[Sauvegardes différentielles](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Sauvegarde des journaux de transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle et ne tronque pas les journaux de transactions.  <br/> |
   
Les composants ou fichiers de base de données, définis par l’auteur du message change représentent les fichiers de base de données et les journaux des transactions dans les bases de données Exchange 2013. Cela permet à votre application de sauvegarde et de restauration afficher les noms des composants au sein d’une base de données Exchange 2013 pendant les opérations de sauvegarde. Votre application de sauvegarde ne peut pas sauvegarder des composants de base de données individuelle, Il peut uniquement sauvegarder les bases de données entière. 
  
Le rédacteur Exchange standardise les chemins de logique de composant de base de données, qui sont spécifiées dans les métadonnées du rédacteur Exchange. Le rédacteur Exchange renvoie les chemins d’accès logiques à votre application de sauvegarde et de restauration selon vos besoins.
  
Le rédacteur Exchange fournit des chemins d’accès logiques sous la forme : 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Les composants serveur et de base de données sont les composants du groupe de fichiers, mais ils n’ont pas tous les fichiers associés. Ils ont sous-composants qui spécifient les fichiers individuels. Une base de données ne contient qu’un seul composant de journal, nommé Logs. Les noms de composant des composants individuels de la base de données sont les GUID des bases de données, affichés sous forme de chaînes. 
  
Le rédacteur Exchange répertorie uniquement les bases de données peuvent être sauvegardées, selon les indications de framework VSS. Bases de données montées en tant que la base de données de récupération Exchange 2013, ainsi que les bases de données qui ne sont pas montées, ne peuvent pas être sauvegardés et par conséquent ne figurent pas dans les métadonnées du rédacteur Exchange.
  
La figure suivante illustre l’enregistreur Exchange processus de sauvegarde. 
  
**La figure 1. Séquence d’événements pour le processus de sauvegarde**

![Diagramme présentant la séquence d’événements pour le processus de sauvegarde. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Sauvegardes complètes
<a name="bk_FullBackups"> </a>

Une sauvegarde complète d’une base de données Exchange implique la création et le stockage d’une copie du fichier de base de données, des journaux des transactions et des fichiers de point de contrôle. Une base de données Exchange 2013 est un ensemble de fichiers journaux des transactions dédié.
  
Une fois que la base de données a été sauvegardée, les fichiers journaux des transactions sur le disque sont tronqués afin que seules les modifications de base de données qui se sont produites après la sauvegarde restent. Pendant ce processus, le rédacteur Exchange supprime toutes les entrées du journal jusqu'à au point de contrôle, basé sur l’hypothèse que les bases de données ont maintenant été sauvegardés dans un état cohérent qui contient toutes les modifications sur le dernier point de contrôle. 
  
Si la base de données en cours de sauvegarde est démontée au cours de l’opération de sauvegarde, Exchange 2013 ne sont pas tronqués les journaux de transactions et le résultat sera l’équivalent d’une opération de sauvegarde copie, pas une opération de sauvegarde complète. 
  
Une sauvegarde complète est terminé, les en-têtes de la base de données montée actif sont mis à jour avec les informations de sauvegarde en cours. Dans les déploiements répliquées, ces informations seront être validé dans un fichier journal de transactions et répliqué sur les autres copies DAG de la base de données. En-têtes des copies de base de données sont mis à jour ce fichier journal des transactions est relu dans la copie de base de données.
  
Une copie de sauvegarde complète VSS est requis pour pouvoir exécuter des sauvegardes de clichés instantanés incrémentielle ou différentielle. Les sauvegardes complètes peuvent provenir d’une copie dans la mesure où il s’agit d’un cliché instantané de sauvegarde.
  
Sauvegardes complètes sont utilisés dans les scénarios suivants :
  
- Une base de données est endommagée ou perdue, mais les fichiers journaux des transactions sur le disque sont intactes. Dans ce scénario, les fichiers de base de données peuvent être restaurés à partir de la sauvegarde complète et puis récupérées par relecture des journaux des transactions sont toujours sur le disque. 
    
- Fichiers journaux des transactions, ainsi que le fichier de base de données sur le disque, est perdu. Dans ce scénario, les fichiers journaux des transactions qui ont été sauvegardés au moment de la sauvegarde complète sont restaurés avec la base de données.
    
Dans Exchange 2013, les journaux peuvent être restaurés sans avoir à restaurer la base de données applicable à partir d’un jeu de sauvegarde complète. Cette option permet une sauvegarde complète précédente être restaurées et combinées avec les fichiers journaux des transactions à partir de la sauvegarde complète la plus récente de reprendre.
  
Lors de l’énumération [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_FULL** lorsque l’auteur du message Exchange effectue une sauvegarde, les composants suivants sont inclus dans la sauvegarde : 
  
- Une base de données avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\> 
    
- Un fichier journal avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\> 
    
## <a name="copy-backups"></a>Copier les sauvegardes
<a name="bk_CopyBackups"> </a>

Une sauvegarde de copie d’une base de données Exchange consiste à créer et stocker les mêmes éléments qui sont inclus dans une sauvegarde complète. Toutefois, contrairement à avec une sauvegarde complète, les fichiers journaux des transactions sur le disque ne sont pas tronqués lors de la sauvegarde est terminée. Les sauvegardes ne sont pas destinés à des fins de récupération de données. Au lieu de cela, les sauvegardes fournissent une image des données à utiliser pour tester, de diagnostiquer les problèmes, ou pour l’amorçage un réplica.
  
Par exemple, un administrateur Exchange 2013 rencontre des problèmes avec la banque Exchange peut-il une copie de sauvegarde à utiliser dans un environnement de test sans affecter le système de production. Les sauvegardes n’affectent pas les plannings de sauvegarde régulières ; Toutefois, car une copie de sauvegarde met également à la banque d’informations Exchange dans un état de la sauvegarde en cours, il bloque les autres sauvegardes planifiées de continuer jusqu'à ce que la copie de sauvegarde est terminée ou annulée. 
  
Lors de l’énumération [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_COPY**, les composants suivants sont inclus dans une copie de sauvegarde : 
  
- Une base de données avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\> 
    
- Un composant du fichier journal avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\>
    
## <a name="incremental-backups"></a>Sauvegardes incrémentielles
<a name="bk_IncrementalBackups"> </a>

Une sauvegarde incrémentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données qui se sont produites depuis la dernière sauvegarde complète ou incrémentielle. Lorsque tous les fichiers de base de données et fichiers journaux sont restaurés au système, ils peuvent être récupérées à leur état au moment de la dernière sauvegarde incrémentielle. Les données stockées dans une sauvegarde incrémentielle incluent uniquement les fichiers journaux des transactions jusqu'à l’heure actuelle. 
  
Une fois la sauvegarde terminée, le serveur Exchange tronque les fichiers journaux et indique l’heure de sauvegarde dans les en-têtes de base de données. À l’aide d’une sauvegarde incrémentielle pour récupérer une base de données nécessite au moins deux ensembles de données à restaurer : la dernière sauvegarde complète, puis chaque sauvegarde incrémentielle effectuée après l’intégralité de la dernière sauvegarde. L’avantage d’utiliser des sauvegardes incrémentielles est que les sauvegardes individuels sont beaucoup plus petits qu’une sauvegarde complète et les sauvegardes incrémentielles individuelles sont souvent plus petites que les sauvegardes différentielles. 
  
L’inconvénient à l’utilisation des sauvegardes incrémentielles, que si le nombre de sauvegardes incrémentielles ont été apportées entre les sauvegardes complètes, récupération de la banque d’informations Exchange peut impliquer des récupération plusieurs sauvegardes incrémentielles. Exchange ne permet pas d’une sauvegarde incrémentielle se produire lorsqu’il n’existe aucune sauvegarde complète précédente pour établir le point de départ pour que les modifications incrémentielles. 
  
Une sauvegarde complète à partir d’un emplacement de copie DAG peut être suivie d’une sauvegarde incrémentielle de l’emplacement actif et vice versa. Une restriction à prendre en compte est que le dernier état de sauvegarde est conservé dans l’en-tête de la base de données active, et les modifications apportées à l’en-tête de la base de données sont écrites dans les journaux de transactions, répliquée et relus à l’emplacement de la base de données copie comme toutes les autres transactions. les journaux dans les déploiements DAG. Étant donné que les sauvegardes et restaurations interagissent, les applications de sauvegarde peuvent fournir les fonctionnalités pour exécuter des sauvegardes exclusivement sur un nœud spécifique de DAG, quel que soit le nœud actif ou passif, ainsi que pour exécuter des sauvegardes en mode exclusif à partir du nœud passif ou en mode exclusif à partir du nœud actif.
  
Lors de l’énumération [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_INCREMENTAL**, les composants suivants sont inclus dans une sauvegarde incrémentielle : 
  
- Une base de données avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\> 
    
- Un fichier journal avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\>
    
## <a name="differential-backups"></a>Sauvegardes différentielles
<a name="bk_DifferentialBackups"> </a>

Une sauvegarde différentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données qui se sont produites depuis la dernière sauvegarde complète ou incrémentielle. Lorsque les fichiers de base de données et les fichiers journaux sont restaurés par le système, ils peuvent être récupérées à l’état à la dernière sauvegarde différentielle. 
  
Les données stockées dans une sauvegarde différentielle incluent uniquement les fichiers journaux des transactions jusqu'à un point de contrôle actuel. Les sauvegardes différentielles ne supprimer ou modifier les fichiers journaux ou modifier les en-têtes de base de données. Pour utiliser une sauvegarde différentielle pour récupérer une base de données, vous devez uniquement restaurer les deux ensembles de données : la dernière sauvegarde complète, puis la sauvegarde différentielle la plus récente. 
  
L’inconvénient à l’utilisation de sauvegardes différentielles, que les sauvegardes différentielles dupliquer la sauvegarde des données dans chaque sauvegarde jusqu'à ce qu’une sauvegarde complète est effectuée. Si plusieurs sauvegardes différentielles sont effectuées entre les sauvegardes complètes, l’espace de stockage requis peut dépasser requis par le même nombre de sauvegardes incrémentielles. Exchange ne permet pas d’une sauvegarde différentielle puisse se déclencher lorsqu’il n’a pas une sauvegarde complète ou incrémentielle pour établir le point de départ pour les sauvegardes différentielles.
  
Une sauvegarde complète à partir de l’emplacement de copie peut être suivie d’une sauvegarde différentielle de l’emplacement actif et vice versa. Une restriction à prendre en compte est que le dernier état de sauvegarde est conservé dans l’en-tête de la base de données active, et les modifications apportées à l’en-tête de la base de données sont écrites dans les journaux de transactions, répliquée et relus à l’emplacement de la base de données copie comme toutes les autres transactions. les journaux dans les déploiements DAG. Étant donné que les sauvegardes et restaurations interagissent, les applications de sauvegarde fournissent les fonctionnalités pour exécuter toutes les sauvegardes exclusivement sur un nœud spécifique de DAG, quel que soit le nœud actif ou passif, ainsi que pour exécuter des sauvegardes en mode exclusif à partir du nœud passif ou en mode exclusif à partir du nœud actif.
  
Lors de l’énumération [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_DIFFERENTIAL**, les composants suivants sont inclus dans une sauvegarde différentielle : 
  
- Une base de données avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\> 
    
- Un fichier journal avec le chemin d’accès logique banque d’informations Exchange Server\Microsoft\\< nom du serveur\>\\< GUID de la base de données\>
    
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Créer la sauvegarde et de restaurer des applications pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Valider l’intégrité des sauvegardes à l’aide l’outil Eseutil dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

