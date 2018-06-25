---
title: Concepts de sauvegarde et de restauration pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Trouvez des informations sur les bases de données Exchange qui vous aideront à créer votre sauvegarde et de restaurer des applications pour Exchange 2013.
ms.openlocfilehash: 5fa62c3d34ffbe8f0bab852c6d41c49220e2883a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754751"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Concepts de sauvegarde et de restauration pour Exchange 2013

Trouvez des informations sur les bases de données Exchange qui vous aideront à créer votre sauvegarde et de restaurer des applications pour Exchange 2013.
  
Avant de créer la sauvegarde et restauration des applications pour Exchange Server 2013, vous devez être familiarisé avec la structure du fichier de base de données Exchange. En utilisant les fichiers de base de données de banque Exchange, vous pouvez sauvegarder les données dans le magasin d’et restaurer ultérieurement si nécessaire. Si vous êtes limité sur l’espace disque, votre administrateur peut implémenter la journalisation circulaire, et cela affecte votre capacité à sauvegarder la base de données. Vous pouvez également tirer parti de la fonctionnalité de base de données de mobilité dans Exchange 2013 pour sauvegarder et restaurer des données Exchange. Mobilité de base de données, en combinaison avec votre application de sauvegarde et restauration, constitue une bonne mesure de redondance pour la récupération d’urgence.

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Fichiers de base de données de la banque d’informations Exchange

Exchange 2013 prend en charge jusqu'à 100 bases de données. Chaque base de données Exchange 2013 contient les fichiers répertoriés dans le tableau suivant. 
  
**Le tableau 1. Fichiers de base de données Exchange 2013**

|Type de fichier|Extension|Description|
|:-----|:-----|:-----|
|Fichier de base de données  <br/> |\*.edb  <br/> |Enregistre toutes les modifications qui ont été validées dans la base de données en mémoire.  <br/> |
|Flux de journaux de transactions  <br/> |\*.log  <br/> |Enregistre les opérations, telles que la création ou la modification d’un message, qui sont validées dans la base de données. Limité à 1 Mo par opération.  <br/> |
|Fichier de point de contrôle  <br/> |\*.chk.  <br/> |Enregistre les transactions journalisées qui ont été écrites dans les fichiers de base de données sur le disque.  <br/> |
   
Exchange 2013 gère un seul ensemble de fichiers journaux des transactions pour chaque base de données. Les journaux de transaction sont importants pour les opérations de sauvegarde et de récupération. Lorsque vous créez une sauvegarde et restaurez d’application qui utilise le Volume Shadow Copy Service (VSS), vous devez vous assurer que vous gérez ces journaux correctement. Pour plus d’informations, consultez [les journaux de transactions et des fichiers de point de contrôle pour la sauvegarde et de restauration dans Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md). Pour sauvegarder une base de données et ses flux de journal, vous devez sauvegarder la totalité du volume qui contient la base de données et les journaux. Troncature de journal se produit uniquement après un état de réussite d’une sauvegarde complète d’un volume ou des dossiers qui contiennent une base de données Exchange.
  
Sur chaque serveur Exchange, vous pouvez monter qu’une seule base de données de récupération à la fois. Vous pouvez accéder à la base de données de récupération à l’aide des applets de commande Exchange Management Shell comme **New-MailboxRestoreRequest**. Pour plus d’informations sur les bases de données de récupération Exchange, voir [Bases de données de récupération](http://technet.microsoft.com/en-us/library/dd876954%28v=exchg.150%29.aspx) sur TechNet. Pour plus d’informations sur les applets de commande Exchange Management Shell, voir [Applets de commande Exchange 2013](http://technet.microsoft.com/en-us/library/bb124413.aspx) sur TechNet. 
  
## <a name="circular-logging"></a>Enregistrement circulaire
<a name="bk_circularlogging"> </a>

Si la capacité de stockage est un problème, votre administrateur peut activer l’enregistrement circulaire. Lorsque la journalisation circulaire est activée, Exchange écrit les journaux de transactions comme d’habitude, mais lorsqu’un fichier de point de contrôle est avancé, la partie inactive du journal des transactions est tronquée. Votre administrateur doit configurer pas les bases de données Exchange 2013 pour utiliser l’enregistrement circulaire si vous souhaitez également utiliser VSS pour activer votre sauvegarde personnalisée et les opérations de restauration. La journalisation circulaire crée les restrictions suivantes : 
  
- S’il est activé pendant l’opération de sauvegarde ou l’opération de récupération, vous ne pouvez pas restaurer des bases de données.
    
- Seules des opérations de récupération point-à-temps sont possibles. Lorsque la journalisation circulaire est activée, vous pouvez supprimer les journaux de transactions dans le même répertoire lorsqu’une base de données est restaurée, bien que ces journaux peuvent faire partie d’une autre base de données Exchange 2013. 
    
- Vous ne pouvez pas effectuer les opérations de sauvegarde incrémentielles ou différentielles. Pour plus d’informations sur ces types de sauvegardes, voir [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md).
    
Si la journalisation circulaire est active, l’administrateur doit désactiver dès que possible pour vous assurer que vos sauvegardes VSS n’échouent. Pour plus d’informations, consultez le billet de blog [enregistrement circulaire Exchange et les sauvegardes VSS](http://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx). 
  
## <a name="exchange-database-mobility"></a>Mobilité de la base de données Exchange
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 autorise la mobilité de base de données améliorer la disponibilité et la fiabilité de boîte aux lettres. Mobilité de la base de données vous permet de créer des copies de votre base de données de la banque Exchange, se déconnecter de la base de données à partir du serveur et le stocker sur un autre serveur. Dans un Exchange 2013 base de données de disponibilité groupe (DAG), plusieurs copies de la base de données sont stockées sur des ordinateurs différents. Lorsqu’une ou plusieurs copies de la base de données sont perdues en raison de la défaillance système ou matériels, les informations des autres copies peuvent être utilisées pour réamorcer la base de données par le biais d’opérations de réplication normal.
  
Pour les opérations de sauvegarde, si les bases de données Exchange 2013 doivent être sauvegardés sont configurés dans un DAG, l’application de sauvegarde contribue à empêcher interférences entre la capture instantanée et les performances du serveur actif en procédant de la capture instantanée sur un des inactifs copie de base de données. Étant donné que les copies de base de données sont synchronisées pour l’essentiel, l’application de sauvegarde peut prendre des captures instantanées à partir de différentes copies de base de données et il reconstruire ultérieurement à partir d’éléments.
  
Le seul moyen de restaurer des bases de données DAG à partir de données de sauvegarde est de restaurer toutes les copies de la base de données avec les mêmes données de sauvegarde. Comme les fichiers journaux de base de données peuvent différer légèrement d’une copie à une autre, la restauration des copies de base de données individuelles à l’aide de données différentes peut empêcher le montage de la base de données.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Les journaux de transactions et des fichiers de point de contrôle pour la sauvegarde et de restauration dans Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Enregistreur Exchange dans Exchange 2013](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Exchange Online et développement Exchange](../exchange-server-development.md) 
- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    

