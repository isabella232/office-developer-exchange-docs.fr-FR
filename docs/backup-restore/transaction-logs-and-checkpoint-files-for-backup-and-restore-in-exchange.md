---
title: Journaux des transactions et fichiers de point de contrôle pour la sauvegarde et la restauration dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Trouvez des informations sur les journaux de transactions et les fichiers de point de contrôle, ainsi que sur leur utilisation pour la Exchange données 2013.
ms.openlocfilehash: ae47c7757a1001f28c467ea58ec87b4ddbc5a5c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513261"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Journaux des transactions et fichiers de point de contrôle pour la sauvegarde et la restauration dans Exchange

Trouvez des informations sur les journaux de transactions et les fichiers de point de contrôle, ainsi que sur leur utilisation pour la Exchange données 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article décrit comment Exchange Server 2013 utilise les journaux des transactions et les fichiers de point de contrôle pour éviter la perte de données. Il est important de connaître ces informations lorsque vous développez des applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service) dans les versions de Windows Server à partir de Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Journaux de transactions Exchange 2013

Exchange 2013 conserve un ensemble unique de fichiers journaux de transactions pour chaque base de données. Une transaction est définie comme toute opération qui modifie l’état ou le contenu de la base de données. Les fichiers journaux des transactions d’une base de données individuelle enregistrent toutes les transactions effectuées sur la base de données. Les enregistrements des transactions sont écrits dans les journaux des transactions avant d’être effectués dans la base de données proprement dite, afin de garantir que toutes les transactions inscrites peuvent être récupérées en cas de défaillance de la base de données. Exchange journaux des transactions de la base de données 2013 sont stockés sur le disque avant que les transactions ne soient enregistrées dans le fichier de base de données. 
  
L’enregistrement des transactions avant la mise à jour de la base de données est appelé journalisation avant écriture. Pour vous assurer que la base de données est correctement revenir à l’état correct, Exchange 2013 écrit les données dans les fichiers de base de données à l’aide d’écritures et de points de contrôle basés sur des pages. Pendant les opérations normales, Exchange stocke d’abord les modifications de base de données dans les journaux des transactions, puis effectue ces modifications sur une copie en mémoire de la base de données. Les journaux des transactions enregistrent le début et la fin de chaque transaction. Cela garantit que des informations suffisantes sont disponibles pour annuler ou annuler ultérieurement des opérations dans la base de données.
  
Lors de la récupération à partir d’erreurs dans lesquelles le fichier de base de données sur le disque est endommagé, mais que les journaux des transactions sont intacts, votre application de restauration doit d’abord restaurer une copie bonne connue du fichier de base de données.
  
Le Exchange relecture les transactions des journaux de transaction précédemment stockés, puis relect toutes les transactions restantes à partir des fichiers journaux des transactions sur disque. Notez que les transactions peuvent parfois être perdues si le système échoue entre le moment où les transactions sont enregistrées dans les journaux des transactions et le moment où elles sont réellement écrites dans les fichiers de base de données. 
  
Régulièrement, le magasin Exchange vérifie l’image de la base de données en mémoire, puis détermine les pages qui ont été modifiées. Le magasin Exchange combine les modifications en attente, puis écrit ces pages dans le fichier de base de données sur disque.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Fichiers de point de contrôle Exchange 2013

Un fichier de point de contrôle enregistre les transactions enregistrées qui ont été écrites dans les fichiers de base de données sur disque. Le point de contrôle est avancé lorsque toutes les pages de base de données qui ont été modifiées par des entrées dans les journaux des transactions sont correctement écrites sur le disque. Étant donné que le fichier de point de contrôle enregistre les transactions qui se retrouvent déjà dans l’image de base de données sur disque, le magasin Exchange doit uniquement relire les transactions qui se sont produites après le point de contrôle. En fonction de la période entre les sauvegardes, cela peut réduire énormément le nombre de transactions qui doivent être relectées dans la base de données en cas de défaillance du système.
  
## <a name="see-also"></a>Voir aussi

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Types d’opérations de sauvegarde Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauration de Exchange bases de données 2013](restoring-exchange-2013-databases.md)
    

