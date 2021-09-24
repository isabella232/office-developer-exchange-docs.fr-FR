---
title: Types d’opérations de sauvegarde Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Trouvez des informations sur les différents types de sauvegardes que vous pouvez effectuer sur vos bases de données de magasin Exchange 2013, y compris les sauvegardes complètes, de copie, incrémentielles et différentielle.
ms.openlocfilehash: 79fcdaa40409ee7cac4df44711c1551946b85ca1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520254"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Types d’opérations de sauvegarde Exchange 2013

Trouvez des informations sur les différents types de sauvegardes que vous pouvez effectuer sur vos bases de données de magasin Exchange 2013, y compris les sauvegardes complètes, de copie, incrémentielles et différentielle.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les différents types de sauvegardes que vous pouvez effectuer sur les bases de données Exchange Server 2013 et sur la façon dont ces sauvegardes affectent les fichiers de base de données. 
  
Les applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service) et le rédacteur Exchange peuvent effectuer les types de sauvegardes répertoriés dans le tableau suivant.
  
**Tableau 1. Types d’opérations de sauvegarde**

|**Type de sauvegarde**|**Description**|
|:-----|:-----|
|[Sauvegardes complètes](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Permet de back up the databases ( \* .edb), transaction logs ( \* .log), checkpoint files ( \* .chk), and then truncates the transaction logs for a specific database.  <br/> |
|[Copier des sauvegardes](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Enregistre la base de données, les journaux de transactions et les fichiers de point de contrôle. Les sauvegardes de copie ne tronquéent pas les journaux de transactions de la base de données.  <br/> |
|[Sauvegardes incrémentielles](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Sauvegarde les journaux de transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle, puis tronque les journaux de transactions.  <br/> |
|[Sauvegardes différentielle](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Sauvegarde les journaux des transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle et ne tronquée pas les journaux de transactions.  <br/> |
   
Les composants, ou fichiers de base de données, définis par le rédacteur Exchange représentent les fichiers de base de données et les journaux de transactions dans Exchange 2013. Cela permet à votre application de sauvegarde et de restauration d’afficher les noms des composants dans une base de données Exchange 2013 pendant les opérations de sauvegarde. Toutefois, votre application de sauvegarde ne peut pas sauvegarder des composants de base de données individuels . il peut uniquement back up whole databases. 
  
Le rédacteur Exchange standardise les chemins logiques du composant de base de données, qui sont spécifiés dans les métadonnées Exchange rédacteur. Le rédacteur Exchange renvoie les chemins d’accès logiques à votre application de sauvegarde et de restauration si nécessaire.
  
Le rédacteur Exchange fournit des chemins logiques sous la forme : 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Les composants serveur et base de données sont des composants de groupe de fichiers, mais ils n’ont aucun fichier associé. Ils ont des sous-ensembles qui spécifient les fichiers individuels. Une base de données ne contient qu’un seul composant de journal, nommé Logs. Les noms des composants des composants de base de données individuels sont les GUID des bases de données, affichés sous la mesure de chaînes. 
  
Le rédacteur Exchange répertorie uniquement les bases de données qui peuvent être backed, en fonction des instructions de l’infrastructure VSS. Les bases de données montées en tant que base de données de récupération Exchange 2013, ainsi que les bases de données qui ne sont pas montées, ne peuvent pas être montées et, par conséquent, ne sont pas répertoriées dans les métadonnées du rédacteur Exchange.
  
La figure suivante illustre le processus Exchange de l’auteur. 
  
**Figure 1. Séquence d’événements pour le processus de sauvegarde**

![Diagramme présentant la séquence d’événements pour le processus de sauvegarde. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Sauvegardes complètes
<a name="bk_FullBackups"> </a>

Une sauvegarde complète d’une base de données Exchange implique la création et le stockage d’une copie du fichier de base de données, des journaux des transactions et des fichiers de point de contrôle. Une base Exchange 2013 contient un ensemble de fichiers journaux de transactions dédiés.
  
Une fois la base de données sauvegarde, les fichiers journaux des transactions sur le disque sont tronqués afin que seules les modifications de base de données qui se sont produites après la sauvegarde restent. Au cours de ce processus, l’enregistreur Exchange supprime toutes les entrées de journal jusqu’au point de contrôle, en fonction de l’hypothèse que les bases de données ont été désormais dans un état cohérent qui contient toutes les modifications jusqu’au point de contrôle le plus récent. 
  
Si la base de données en cours de sauvegarde est démontée pendant l’opération de sauvegarde, Exchange 2013 ne tronquée pas les journaux des transactions et le résultat équivaut à une opération de sauvegarde de copie, et non à une opération de sauvegarde complète. 
  
Lorsqu’une sauvegarde complète est terminée, les en-têtes de la base de données montée active sont mis à jour avec les informations de sauvegarde actuelles. Dans les déploiements répliqués, ces informations sont committedes dans un fichier journal des transactions et répliquées dans les autres copies DAG de la base de données. Les en-têtes des copies de base de données sont mis à jour lorsque ce fichier journal des transactions est relecture dans la copie de base de données.
  
Une sauvegarde complète du shadow copy est nécessaire pour exécuter des sauvegardes de copies de secours incrémentielles ou différentielle. Les sauvegardes complètes peuvent être prises à partir de n’importe quelle copie tant qu’il s’agit d’une sauvegarde de copie de secours.
  
Les sauvegardes complètes sont utilisées dans les scénarios suivants :
  
- Une base de données est endommagée ou perdue, mais les fichiers journaux des transactions sur le disque sont intacts. Dans ce scénario, les fichiers de base de données affectés peuvent être restaurés à partir de la sauvegarde complète, puis récupérés en relisant les journaux de transactions qui sont encore sur le disque. 
    
- Les fichiers journaux des transactions, ainsi que le fichier de base de données sur disque, sont perdus. Dans ce scénario, les fichiers journaux des transactions qui ont été sauvegardes au moment de la sauvegarde complète sont restaurés avec la base de données.
    
Dans Exchange 2013, les journaux peuvent être restaurés sans avoir à restaurer la base de données applicable à partir d’un jeu de sauvegarde complet. Cette option permet de restaurer et de combiner une sauvegarde complète précédente avec les fichiers journaux des transactions de la sauvegarde complète la plus récente.
  
Lorsque [l’VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_FULL** lorsque le rédacteur Exchange effectue une sauvegarde, les composants suivants sont inclus dans la sauvegarde : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Nom de la base de \\ données<'informations Microsoft<base \> \\ de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Nom de la base de données<de la banque d’informations Microsoft<de \\ \> \\ données\> 
    
## <a name="copy-backups"></a>Copier des sauvegardes
<a name="bk_CopyBackups"> </a>

Une sauvegarde de copie d’Exchange base de données implique la création et le stockage des mêmes éléments inclus dans une sauvegarde complète. Toutefois, contrairement à une sauvegarde complète, les fichiers journaux des transactions sur le disque ne sont pas tronqués lorsque la sauvegarde est terminée. Les sauvegardes de copie ne sont pas destinées à des fins de récupération de données. Au lieu de cela, les sauvegardes de copie fournissent une image des données à utiliser dans le test, le diagnostic des problèmes ou l’amorçage d’un réplica.
  
Par exemple, un administrateur Exchange 2013 qui rencontre des problèmes avec le magasin Exchange peut effectuer une sauvegarde de copie à utiliser dans un environnement de test sans affecter le système de production. Les sauvegardes de copie n’affectent pas les planifications de sauvegarde normales ; toutefois, étant donné qu’une sauvegarde de copie place également le magasin Exchange dans un état de sauvegarde en cours, elle empêche les autres sauvegardes programmées de se poursuivre jusqu’à ce que la sauvegarde de copie soit terminée ou abandonnée. 
  
Lorsque [l’VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_COPY,** les composants suivants sont inclus dans une sauvegarde de copie : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Nom de la base de \\ données<'informations Microsoft<base \> \\ de données\> 
    
- Composant de fichier journal avec le chemin d’accès logique Exchange Server\Nom du serveur de la banque d’informations Microsoft \\<nom de<base \> \\ de données\>
    
## <a name="incremental-backups"></a>Sauvegardes incrémentielles
<a name="bk_IncrementalBackups"> </a>

Une sauvegarde incrémentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données depuis la dernière sauvegarde complète ou incrémentielle. Lorsque tous les fichiers de base de données et les fichiers journaux sont restaurés dans le système, ils peuvent être récupérés à l’état où ils étaient au moment de la dernière sauvegarde incrémentielle. Les données stockées dans une sauvegarde incrémentielle incluent uniquement les fichiers journaux des transactions jusqu’à l’heure actuelle. 
  
Une fois la sauvegarde terminée, le serveur Exchange tronque les fichiers journaux et marque l’heure de sauvegarde dans les en-têtes de base de données. L’utilisation d’une sauvegarde incrémentielle pour récupérer une base de données nécessite au moins deux jeux de données à restaurer : la dernière sauvegarde complète, puis chaque sauvegarde incrémentielle prise après la dernière sauvegarde complète. L’avantage d’utiliser des sauvegardes incrémentielles est que les sauvegardes individuelles sont beaucoup plus petites qu’une sauvegarde complète et que les sauvegardes incrémentielles individuelles sont souvent plus petites que les sauvegardes différentielle. 
  
L’inconvénient de l’utilisation de sauvegardes incrémentielles est que si de nombreuses sauvegardes incrémentielles ont été réalisées entre des sauvegardes complètes, la récupération du magasin Exchange peut impliquer la récupération de nombreuses sauvegardes incrémentielles. Exchange n’autorise pas une sauvegarde incrémentielle lorsqu’il n’existe aucune sauvegarde complète précédente pour établir le point de départ des modifications incrémentielles. 
  
Une sauvegarde complète provenant d’un emplacement de copie DAG peut être suivie d’une sauvegarde incrémentielle à partir de l’emplacement actif et vice versa. Une restriction à garder à l’esprit est que la dernière sauvegarde est conservée dans l’en-tête de la base de données active et que les modifications apportées à l’en-tête de base de données sont écrites dans les journaux des transactions, répliquées et relectées à l’emplacement de la base de données de copie, comme tous les autres journaux de transactions dans les déploiements DAG. Étant donné que les sauvegardes et les restaurations interopérables, les applications de sauvegarde peuvent fournir la fonctionnalité d’exécuter des sauvegardes exclusivement sur un nœud DAG spécifique, que le nœud soit actif ou passif, et qu’il exécute des sauvegardes exclusivement à partir du nœud passif ou exclusivement à partir du nœud actif.
  
Lorsque [l’VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_INCREMENTAL,** les composants suivants sont inclus dans une sauvegarde incrémentielle : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Nom de la base de \\ données<'informations Microsoft<base \> \\ de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Nom de la base de données<de la banque d’informations Microsoft<de \\ \> \\ données\>
    
## <a name="differential-backups"></a>Sauvegardes différentielle
<a name="bk_DifferentialBackups"> </a>

Une sauvegarde différentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données depuis la dernière sauvegarde complète ou incrémentielle. Lorsque les fichiers de base de données et les fichiers journaux sont restaurés par le système, ils peuvent être récupérés à l’état où ils se trouveraient lors de la dernière sauvegarde différentielle. 
  
Les données stockées dans une sauvegarde différentielle incluent uniquement les fichiers journaux des transactions jusqu’au point de contrôle actuel. Les sauvegardes différentielle ne suppriment ni ne modifient les fichiers journaux, ni ne modifient les en-têtes de base de données. Pour utiliser une sauvegarde différentielle pour récupérer une base de données, il vous suffit de restaurer deux jeux de données : la dernière sauvegarde complète, puis la sauvegarde différentielle la plus récente. 
  
L’inconvénient de l’utilisation des sauvegardes différentielle est que les sauvegardes différentielle dupliquent les données de chaque sauvegarde jusqu’à ce qu’une sauvegarde complète soit effectuée. Si de nombreuses sauvegardes différentielle sont prises entre des sauvegardes complètes, l’espace de stockage requis peut dépasser celui requis par le même nombre de sauvegardes incrémentielles. Exchange n’autorise pas une sauvegarde différentielle lorsqu’il n’y a pas eu de sauvegarde complète ou incrémentielle pour établir le point de départ des sauvegardes différentielle.
  
Une sauvegarde complète provenant de l’emplacement de copie peut être suivie d’une sauvegarde différentielle à partir de l’emplacement actif et vice versa. Une restriction à garder à l’esprit est que la dernière sauvegarde est conservée dans l’en-tête de la base de données active et que les modifications apportées à l’en-tête de base de données sont écrites dans les journaux des transactions, répliquées et relectées à l’emplacement de la base de données de copie, comme tous les autres journaux de transactions dans les déploiements DAG. Étant donné que les sauvegardes et les restaurations interopérables, les applications de sauvegarde fournissent la fonctionnalité d’exécuter toutes les sauvegardes exclusivement sur un nœud DAG spécifique, que le nœud soit actif ou passif, et qu’il exécute des sauvegardes exclusivement à partir du nœud passif ou exclusivement à partir du nœud actif.
  
Lorsque [l’VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_DIFFERENTIAL,** les composants suivants sont inclus dans une sauvegarde différentielle : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Nom de la base de \\ données<'informations Microsoft<base \> \\ de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Nom de la base de données<de la banque d’informations Microsoft<de \\ \> \\ données\>
    
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restauration de Exchange bases de données 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validation de l’intégrité de la sauvegarde à l’aide de l’outil Eseutil Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

