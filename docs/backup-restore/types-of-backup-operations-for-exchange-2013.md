---
title: Types d’opérations de sauvegarde pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Trouvez des informations sur les différents types de sauvegarde que vous pouvez effectuer sur vos bases de données de banque Exchange 2013, notamment les sauvegardes complètes, copiées, incrémentielles et différentielles.
ms.openlocfilehash: dd07226acb3a3bb055e98f861a5c01375ee50dda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456285"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Types d’opérations de sauvegarde pour Exchange 2013

Trouvez des informations sur les différents types de sauvegarde que vous pouvez effectuer sur vos bases de données de banque Exchange 2013, notamment les sauvegardes complètes, copiées, incrémentielles et différentielles.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les différents types de sauvegardes que vous pouvez effectuer sur les bases de données Exchange Server 2013 et sur la façon dont ces sauvegardes affectent les fichiers de base de données. 
  
Les applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service) et le rédacteur Exchange peuvent effectuer les types de sauvegardes indiquées dans le tableau suivant.
  
**Tableau 1. Types d’opérations de sauvegarde**

|**Type de sauvegarde**|**Description**|
|:-----|:-----|
|[Sauvegardes complètes](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Sauvegarde les bases de données ( \* . edb), journaux de transactions ( \* . log), fichiers de point de contrôle ( \* . chk), puis tronque les journaux de transaction pour une base de données spécifique.  <br/> |
|[Sauvegardes de copie](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Sauvegarde la base de données, les journaux de transaction et les fichiers de point de contrôle. Les sauvegardes de copie ne tronquent pas les journaux de transactions de la base de données.  <br/> |
|[Sauvegardes incrémentielles](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Sauvegarde les journaux de transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle, puis tronque les journaux de transactions.  <br/> |
|[Sauvegardes différentielles](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Sauvegarde les journaux de transactions pour enregistrer les modifications apportées depuis la dernière sauvegarde complète ou incrémentielle et ne tronque pas les journaux de transactions.  <br/> |
   
Les composants, ou fichiers de base de données, définis par l’enregistreur Exchange représentent les fichiers de base de données et les journaux de transactions dans les bases de données Exchange 2013. Cela permet à votre application de sauvegarde et de restauration d’afficher les noms des composants dans une base de données Exchange 2013 lors des opérations de sauvegarde. Votre application de sauvegarde ne peut pas sauvegarder des composants de base de données individuels ; Il peut uniquement sauvegarder des bases de données entières. 
  
Le writer Exchange normalise les chemins logiques des composants de base de données, qui sont spécifiés dans les métadonnées de l’enregistreur Exchange. Le rédacteur Exchange renvoie les chemins logiques à votre application de sauvegarde et de restauration selon vos besoins.
  
L’enregistreur Exchange fournit des chemins d’accès logiques sous la forme : 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Les composants serveur et base de données sont des composants de groupe de fichiers, mais ils ne sont associés à aucun fichier. Elles possèdent des sous-composants qui spécifient les fichiers individuels. Une base de données contient un seul composant de journal nommé logs. Les noms de composants des composants de base de données individuels sont les GUID des bases de données, présentés sous forme de chaînes. 
  
L’enregistreur Exchange répertorie uniquement les bases de données qui peuvent être sauvegardées, en fonction des instructions de l’infrastructure VSS. Les bases de données qui sont montées en tant que base de données de récupération Exchange 2013, ainsi que les bases de données qui ne sont pas montées, ne peuvent pas être sauvegardées et, par conséquent, ne sont pas répertoriées dans les métadonnées de l’enregistreur Exchange.
  
La figure suivante illustre le processus de sauvegarde du rédacteur Exchange. 
  
**Figure 1. Séquence d’événements pour le processus de sauvegarde**

![Diagramme présentant la séquence d’événements pour le processus de sauvegarde. La séquence commence avec le démarrage de la banque d’informations Exchange, puis continue à travers de nombreuses étapes entre l’enregistreur Exchange, VSS et l’application cliente.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Sauvegardes complètes
<a name="bk_FullBackups"> </a>

Une sauvegarde complète d’une base de données Exchange implique la création et le stockage d’une copie du fichier de base de données, des journaux de transaction et des fichiers de point de contrôle. Une base de données Exchange 2013 possède un ensemble de fichiers journaux de transactions dédiés.
  
Une fois la base de données sauvegardée, les fichiers journaux des transactions sur le disque sont tronqués de sorte que seules les modifications de la base de données qui ont eu lieu après la sauvegarde sont conservées. Pendant ce processus, l’enregistreur Exchange supprime toutes les entrées du journal jusqu’au point de contrôle, en partant du principe que les bases de données ont été sauvegardées dans un état cohérent qui contient toutes les modifications apportées au dernier point de contrôle. 
  
Si la base de données en cours de sauvegarde est démontée pendant l’opération de sauvegarde, Exchange 2013 ne tronque pas les journaux de transactions et le résultat est l’équivalent d’une opération de sauvegarde de copie, et non d’une opération de sauvegarde complète. 
  
Lorsqu’une sauvegarde complète est terminée, les en-têtes de la base de données montée active sont mis à jour avec les informations de sauvegarde actuelles. Dans les déploiements répliqués, ces informations sont validées dans un fichier journal des transactions et répliquées dans les autres copies DAG de la base de données. Les en-têtes des copies de base de données sont mis à jour, car ce fichier journal des transactions est relu dans la copie de base de données.
  
Une sauvegarde de clichés instantanés complète est nécessaire pour exécuter des sauvegardes de clichés instantanés incrémentielles ou différentielles. Les sauvegardes complètes peuvent être effectuées à partir de n’importe quelle copie tant qu’il s’agit d’une sauvegarde de clichés instantanés.
  
Les sauvegardes complètes sont utilisées dans les scénarios suivants :
  
- Une base de données est endommagée ou perdue, mais les fichiers journaux des transactions sur le disque sont intacts. Dans ce scénario, les fichiers de base de données concernés peuvent être restaurés à partir de la sauvegarde complète, puis récupérés en relisant les journaux de transactions qui se trouvent toujours sur le disque. 
    
- Les fichiers journaux de transactions, ainsi que le fichier de base de données sur le disque, sont perdus. Dans ce scénario, les fichiers journaux des transactions sauvegardés au moment de la sauvegarde complète sont restaurés avec la base de données.
    
Dans Exchange 2013, les journaux peuvent être restaurés sans qu’il soit nécessaire de restaurer la base de données applicable à partir d’un jeu de sauvegarde complète. Cette option permet de restaurer une sauvegarde complète précédente et de la combiner avec les fichiers journaux des transactions de la sauvegarde complète la plus récente pour la restaurer vers l’avant.
  
Lorsque l’énumération [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_FULL** lorsque le rédacteur Exchange effectue une sauvegarde, les composants suivants sont inclus dans la sauvegarde : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\> 
    
## <a name="copy-backups"></a>Sauvegardes de copie
<a name="bk_CopyBackups"> </a>

Une sauvegarde de copie d’une base de données Exchange implique la création et le stockage des mêmes éléments inclus dans une sauvegarde complète. Toutefois, contrairement à une sauvegarde complète, les fichiers journaux des transactions sur le disque ne sont pas tronqués une fois la sauvegarde terminée. Les sauvegardes de copie ne sont pas destinées à la récupération des données. Au lieu de cela, les sauvegardes de copie fournissent une image des données à utiliser dans les tests, le diagnostic du problème ou pour l’amorçage d’un réplica.
  
Par exemple, un administrateur Exchange 2013 qui rencontre des problèmes avec la Banque d’aide Exchange peut faire une sauvegarde de copie pour une utilisation dans un environnement de test sans affecter le système de production. Les sauvegardes de copie n’affectent pas les planifications de sauvegarde régulières ; Toutefois, dans la mesure où une sauvegarde de copie place également la Banque d’Exchange dans un état de sauvegarde en cours d’exécution, elle bloque les autres sauvegardes planifiées jusqu’à ce que la sauvegarde de copie soit terminée ou abandonnée. 
  
Lorsque l’énumération [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_COPY**, les composants suivants sont inclus dans une sauvegarde de copie : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\> 
    
- Un composant de fichier journal avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\>
    
## <a name="incremental-backups"></a>Sauvegardes incrémentielles
<a name="bk_IncrementalBackups"> </a>

Une sauvegarde incrémentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données depuis la dernière sauvegarde complète ou incrémentielle. Lorsque tous les fichiers de base de données et les fichiers journaux sont restaurés sur le système, ils peuvent être restaurés à l’État dans lequel ils se trouvaient au moment de la dernière sauvegarde incrémentielle. Les données stockées dans une sauvegarde incrémentielle incluent uniquement les fichiers journaux des transactions jusqu’à l’heure actuelle. 
  
Une fois la sauvegarde terminée, le serveur Exchange tronque les fichiers journaux et marque l’heure de la sauvegarde dans les en-têtes de la base de données. L’utilisation d’une sauvegarde incrémentielle pour récupérer une base de données nécessite la restauration d’au moins deux ensembles de données : la dernière sauvegarde complète, puis chaque sauvegarde incrémentielle effectuée après la dernière sauvegarde complète. L’avantage d’utiliser des sauvegardes incrémentielles est que les sauvegardes individuelles sont bien plus petites qu’une sauvegarde complète et que les sauvegardes incrémentielles individuelles sont souvent plus petites que les sauvegardes différentielles. 
  
L’inconvénient d’utiliser des sauvegardes incrémentielles est que si plusieurs sauvegardes incrémentielles ont été effectuées entre les sauvegardes complètes, la restauration de la Banque d’Exchange peut impliquer la restauration de nombreuses sauvegardes incrémentielles. Exchange n’autorise pas la sauvegarde incrémentielle lorsqu’il n’existe pas de sauvegarde complète précédente pour établir le point de départ pour les modifications incrémentielles. 
  
Une sauvegarde complète effectuée à partir d’un emplacement de copie DAG peut être suivie d’une sauvegarde incrémentielle à partir de l’emplacement actif et vice versa. L’une des restrictions à garder à l’esprit est que le dernier état de sauvegarde est conservé dans l’en-tête de la base de données active, et les modifications apportées à l’en-tête de la base de données sont écrites dans les journaux de transactions, répliquées et relues à l’emplacement de la base de données comme tous les autres journaux de transactions dans les déploiements DAG Étant donné que les sauvegardes et les restaurations interagissent, les applications de sauvegarde peuvent fournir la fonctionnalité permettant d’exécuter des sauvegardes exclusivement sur un nœud DAG spécifique, que le nœud soit actif ou passif, ainsi que d’exécuter des sauvegardes exclusivement à partir du nœud passif ou exclusivement à partir du nœud actif.
  
Lorsque l’énumération [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_INCREMENTAL**, les composants suivants sont inclus dans une sauvegarde incrémentielle : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\>
    
## <a name="differential-backups"></a>Sauvegardes différentielles
<a name="bk_DifferentialBackups"> </a>

Une sauvegarde différentielle d’une base de données Exchange 2013 enregistre les modifications apportées à la base de données depuis la dernière sauvegarde complète ou incrémentielle. Lorsque les fichiers de base de données et les fichiers journaux sont restaurés par le système, ils peuvent être récupérés à l’État dans lequel ils se trouvaient à la dernière sauvegarde différentielle. 
  
Les données stockées dans une sauvegarde différentielle incluent uniquement les fichiers journaux des transactions jusqu’au point de contrôle actuel. Les sauvegardes différentielles ne suppriment pas les fichiers journaux ou ne modifient pas les en-têtes de base de données. Pour utiliser une sauvegarde différentielle afin de récupérer une base de données, il vous suffit de restaurer deux jeux de données : la dernière sauvegarde complète, puis la sauvegarde différentielle la plus récente. 
  
L’inconvénient d’utiliser des sauvegardes différentielles est que les sauvegardes différentielles dupliquent les données sauvegardées dans chaque sauvegarde jusqu’à ce qu’une sauvegarde complète soit effectuée. Si de nombreuses sauvegardes différentielles sont effectuées entre les sauvegardes complètes, l’espace de stockage requis peut être supérieur à celui requis par le même nombre de sauvegardes incrémentielles. Exchange n’autorise pas la sauvegarde différentielle lorsqu’il n’y a pas eu une sauvegarde complète ou incrémentielle pour établir le point de départ des sauvegardes différentielles.
  
Une sauvegarde complète effectuée à partir de l’emplacement de la copie peut être suivie d’une sauvegarde différentielle à partir de l’emplacement actif et vice versa. L’une des restrictions à garder à l’esprit est que le dernier état de sauvegarde est conservé dans l’en-tête de la base de données active, et les modifications apportées à l’en-tête de la base de données sont écrites dans les journaux de transactions, répliquées et relues à l’emplacement de la base de données comme tous les autres journaux de transactions dans les déploiements DAG Étant donné que les sauvegardes et les restaurations interagissent, les applications de sauvegarde offrent la possibilité d’exécuter toutes les sauvegardes exclusivement sur un nœud DAG spécifique, que le nœud soit actif ou passif, ainsi que d’exécuter des sauvegardes exclusivement à partir du nœud passif ou exclusivement à partir du nœud actif.
  
Lorsque l’énumération [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) dans VSS est définie sur **VSS_BT_DIFFERENTIAL**, les composants suivants sont inclus dans une sauvegarde différentielle : 
  
- Une base de données avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\> 
    
- Un fichier journal avec le chemin d’accès logique Exchange Server\Microsoft Information \\<Store nom du serveur \> \\<GUID de base de données\>
    
## <a name="see-also"></a>Voir aussi
<a name="bk_AdditionalResources"> </a>

- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’outil Eseutil dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

