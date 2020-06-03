---
title: Journaux de transaction et fichiers de point de contrôle pour la sauvegarde et la restauration dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Trouvez des informations sur les journaux de transaction et les fichiers de point de contrôle et la façon dont ils sont utilisés pour sauvegarder et restaurer les données Exchange 2013.
ms.openlocfilehash: 5b01fc6924f82e76943795df877ae84b1fde087b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456387"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Journaux de transaction et fichiers de point de contrôle pour la sauvegarde et la restauration dans Exchange

Trouvez des informations sur les journaux de transaction et les fichiers de point de contrôle et la façon dont ils sont utilisés pour sauvegarder et restaurer les données Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article explique comment Exchange Server 2013 utilise les journaux de transaction et les fichiers de point de contrôle pour éviter toute perte de données. Il est important de connaître ces informations lorsque vous développez des applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service) dans les versions de Windows Server à partir de Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Journaux de transactions dans Exchange 2013

Exchange 2013 gère un seul ensemble de fichiers journaux de transactions pour chaque base de données. Une transaction est définie comme n’importe quelle opération qui modifie l’État ou le contenu de la base de données. Les fichiers journaux des transactions d’une base de données individuelle enregistrent toutes les transactions effectuées sur la base de données. Les enregistrements des transactions sont écrits dans les journaux des transactions avant d’être créés dans la base de données proprement dite, afin de s’assurer que toutes les transactions validées peuvent être récupérées en cas de défaillance de la base de données. Les journaux de transaction de base de données Exchange 2013 sont stockés sur le disque avant la validation des transactions dans le fichier de base de données. 
  
L’enregistrement des transactions avant la mise à jour de la base de données est appelé journalisation en écriture anticipée. Pour vous assurer que la base de données est correctement ramenée à l’état correct, Exchange 2013 écrit des données dans les fichiers de base de données à l’aide d’écritures et de points de contrôle basés sur la page. Pendant les opérations normales, la Banque d’données Exchange enregistre d’abord les modifications apportées à la base de données dans les journaux de transactions, puis apporte ces modifications sur une copie en mémoire de la base de données. Les journaux de transaction enregistrent le début et la fin de chaque transaction. Cela garantit que des informations suffisantes sont disponibles pour annuler ou restaurer ultérieurement les opérations dans la base de données.
  
Lors de la récupération d’erreurs dans le cas où le fichier de base de données sur le disque est endommagé, mais que les journaux de transactions sont intacts, votre application de restauration doit d’abord restaurer une copie correcte connue du fichier de base de données.
  
La banque Exchange relit les transactions à partir des journaux de transactions sauvegardés précédemment, puis relit les transactions restantes des fichiers journaux de transactions sur disque. Notez que parfois, les transactions peuvent être perdues si le système échoue entre le moment où les transactions sont enregistrées dans les journaux de transactions et quand elles sont effectivement écrites dans les fichiers de base de données. 
  
Régulièrement, la Banque d’Exchange vérifie l’image de base de données en mémoire, puis détermine les pages qui ont été modifiées. La banque Exchange combine les modifications en attente, puis écrit ces pages dans le fichier de base de données sur le disque.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Fichiers de point de contrôle dans Exchange 2013

Un fichier de point de contrôle enregistre les transactions journalisées qui ont été écrites dans les fichiers de base de données sur le disque. Le point de contrôle est avancé lorsque toutes les pages de base de données qui ont été modifiées par des entrées dans les journaux de transactions sont correctement écrites sur le disque. Étant donné que le fichier de point de contrôle enregistre les transactions qui se trouvent déjà dans l’image de la base de données sur le disque, la banque Exchange n’a besoin que de relire les transactions survenues après le point de contrôle. En fonction de la période entre les sauvegardes, cela peut réduire considérablement le nombre de transactions qui doivent être lues dans la base de données en cas de défaillance du système.
  
## <a name="see-also"></a>Voir aussi

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    

