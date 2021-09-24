---
title: Concepts de sauvegarde et de restauration pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Trouvez des informations sur Exchange de données qui vous aideront à créer vos applications de sauvegarde et de restauration pour Exchange 2013.
ms.openlocfilehash: c0b2e0269c3668779f980bf6984d84aff76573f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510518"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Concepts de sauvegarde et de restauration pour Exchange 2013

Trouvez des informations sur Exchange de données qui vous aideront à créer vos applications de sauvegarde et de restauration pour Exchange 2013.
  
Avant de créer des applications de sauvegarde et de restauration pour Exchange Server 2013, vous devez connaître la structure de Exchange base de données. En utilisant les fichiers de base de données de magasin Exchange, vous pouvez sauvegarder les données dans votre banque d’informations et les restaurer ultérieurement selon vos besoins. Si vous êtes limité par l’espace disque, votre administrateur peut mettre en œuvre un enregistrement circulaire mais cela affectera votre capacité à sauvegarder la base de données. Vous pouvez également tirer parti de la fonctionnalité de mobilité de base de données Exchange 2013 pour restaurer et Exchange données. La mobilité de base de données combinée à l’application de sauvegarde et restauration est une bonne solution de redondance en vue d’une récupération d’urgence.

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Fichiers de base de données de la banque d’informations Exchange

Exchange 2013 inclut la prise en charge de 100 bases de données au plus. Chaque Exchange base de données 2013 contient les fichiers répertoriés dans le tableau suivant. 
  
**Tableau 1. Exchange de base de données 2013**

|Type de fichier|Extension|Description|
|:-----|:-----|:-----|
|Fichier de base de données  <br/> |\*.edb  <br/> |Enregistre toutes les modifications qui ont été validées dans la base de données en mémoire.  <br/> |
|Flux de journaux de transactions  <br/> |\*.log  <br/> |Enregistre les opérations, telles que la création ou la modification d’un message, qui sont validées dans la base de données. Limité à 1 Mo par opération.  <br/> |
|Fichier de point de contrôle  <br/> |\*.chk  <br/> |Enregistre les transactions journalisées qui ont été écrites dans les fichiers de base de données sur le disque.  <br/> |
   
Exchange 2013 conserve un ensemble unique de fichiers journaux de transactions pour chaque base de données. Les journaux de transaction sont importants pour les opérations de sauvegarde et de récupération. Lorsque vous créez une sauvegarde et restaurez une application qui utilise le service VSS (Volume Shadow Copy Service), vous devez vous assurer de gérer ces journaux correctement. Pour plus d’informations, reportez-vous à la rubrique [Journaux de transactions et fichiers de point de contrôle de sauvegarde et de restauration dans Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md). Pour sauvegarder une base de données et son flux de journal, vous devez sauvegarder le volume entier qui les contient. La troncature des journaux se produit uniquement après l’exécution d’une sauvegarde complète d’un volume ou de dossiers contenant une base de données Exchange.
  
Sur chaque serveur Exchange, vous ne pouvez monter qu’une base de données de récupération à la fois. Vous pouvez accéder à la base de données de récupération en utilisant les applets de commande Exchange Management Shell comme **New-MailboxRestoreRequest**. Pour plus d’informations sur Exchange de récupération, voir [Bases de](https://technet.microsoft.com/library/dd876954%28v=exchg.150%29.aspx) données de récupération sur TechNet. Pour plus d’informations Exchange cmdlets Management Shell, voir [Exchange 2013 Cmdlets](https://technet.microsoft.com/library/bb124413.aspx) sur TechNet. 
  
## <a name="circular-logging"></a>Enregistrement circulaire
<a name="bk_circularlogging"> </a>

Si la capacité de stockage est un problème, votre administrateur peut activer l’enregistrement circulaire. Lorsque l’enregistrement circulaire est activé, Exchange écrit les journaux de transaction normalement, mais lorsqu’un fichier de point de contrôle est avancé, la partie inactive du journal des transactions est tronquée. Votre administrateur ne doit pas configurer Exchange 2013 pour utiliser la journalisation circulaire si vous envisagez également d’utiliser VSS pour activer vos opérations de sauvegarde et de restauration personnalisées. L’enregistrement circulaire induit les restrictions suivantes : 
  
- S’il est activé pendant l’opération de sauvegarde ou l’opération de récupération, vous ne pouvez pas restaurer des bases de données.
    
- Seules les opérations de récupération jusqu’à une date et heure sont possibles. Lorsque l’enregistrement circulaire est activé, vous pouvez supprimer les journaux des transactions dans le même répertoire lorsqu’une base de données est restaurée, bien que ces journaux peuvent faire partie d’une base de données Exchange 2013 différente. 
    
- Vous ne pouvez pas effectuer des opérations de sauvegarde incrémentielle ou différentielle. Pour plus d’informations sur ces types de sauvegardes, voir Types d’opérations de [sauvegarde Exchange 2013.](types-of-backup-operations-for-exchange-2013.md)
    
Si l’enregistrement circulaire est activé, votre administrateur doit le désactiver dès que possible pour vous assurer que vos sauvegardes VSS n’échouent pas. Pour plus d’informations, consultez le billet de blog Exchange journalisation circulaire [et les sauvegardes VSS.](https://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx) 
  
## <a name="exchange-database-mobility"></a>Mobilité de la base de données Exchange
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 permet la mobilité des bases de données pour améliorer la fiabilité et la disponibilité des boîtes aux lettres. La mobilité de base de données vous permet de créer des copies de votre base de données Exchange, de déconnecter la base de données du serveur et de la stocker sur un autre serveur. Dans un Exchange groupe de disponibilité de base de données (DAG) 2013, plusieurs copies de la base de données sont stockées sur différents ordinateurs. Lorsqu’une ou plusieurs copies de la base de données sont perdues en raison d’une panne matérielle ou système, les informations des autres copies peuvent être utilisées pour réamorcer la base de données par le biais d’opérations de réplication normale.
  
Pour les opérations de sauvegarde, si les bases de données Exchange 2013 à sauvegarder sont configurées dans un DAG, l’application de sauvegarde peut mieux éviter les interférences entre la capture instantanée et les performances du serveur actif en prenant la capture instantanée sur l’une des copies de base de données inactives. Étant donné que les copies de base de données sont synchronisées dans la plupart des cas, l’application de sauvegarde peut prendre des instantanés de différentes versions de la base de données et la recréer ultérieurement à partir de ces éléments.
  
Le seul moyen de restaurer des bases de données DAG à partir de données de sauvegarde est de restaurer toutes les copies de la base de données avec les mêmes données de sauvegarde. Comme les fichiers journaux de base de données peuvent différer légèrement d’une copie à une autre, la restauration des copies de base de données individuelles à l’aide de données différentes peut empêcher le montage de la base de données.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Journaux des transactions et fichiers de point de contrôle pour la sauvegarde et la restauration Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange rédacteur en Exchange 2013](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Développement d’Exchange et Exchange Online](../exchange-server-development.md) 
- [Types d’opérations de sauvegarde Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauration de Exchange bases de données 2013](restoring-exchange-2013-databases.md)
    

