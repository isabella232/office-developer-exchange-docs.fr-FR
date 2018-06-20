---
title: Les journaux de transactions et des fichiers de point de contrôle pour la sauvegarde et de restauration dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Trouvez des informations sur les journaux de transactions et des fichiers de point de contrôle et comment ils sont utilisés pour sauvegarder et restaurer des données Exchange 2013.
ms.openlocfilehash: 53f128348bb2e8895bc1eefaf62402fa348c81ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754772"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Les journaux de transactions et des fichiers de point de contrôle pour la sauvegarde et de restauration dans Exchange

Trouvez des informations sur les journaux de transactions et des fichiers de point de contrôle et comment ils sont utilisés pour sauvegarder et restaurer des données Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article décrit comment Exchange Server 2013 utilise les journaux de transactions et des fichiers de point de contrôle pour éviter les pertes de données. Il est important de connaître ces informations lorsque vous développez de sauvegarde et la restaurez des applications qui utilisent le Volume Shadow Copy Service (VSS) dans les versions de Windows Server à partir de Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Journaux des transactions dans Exchange 2013

Exchange 2013 gère un seul ensemble de fichiers journaux des transactions pour chaque base de données. Une transaction est définie en tant que toute opération qui modifie l’état ou le contenu de la base de données. Les fichiers journaux des transactions pour un enregistrement de base de données individuelle toutes les transactions effectuées sur la base de données. Enregistrements des transactions sont écrites dans les journaux de transactions avant d’être rendues dans la base de données, pour s’assurer que toutes les transactions validées peuvent être récupérées en cas de défaillance de base de données. Journaux de transactions de base de données Exchange 2013 sont stockés sur le disque avant des transactions sont validées dans le fichier de base de données. 
  
L’enregistrement des transactions avant la mise à jour de la base de données est appelé journalisation préalable. Pour garantir que la base de données est correctement remis à l’état approprié, Exchange 2013 écrit des données dans les fichiers de base de données à l’aide de points de contrôle et les écritures basée sur une page. Lors d’opérations habituelles, la banque d’informations Exchange enregistre tout d’abord la base de données dans les journaux de transactions, puis, ces modifications sont effectuées sur une copie en mémoire de la base de données. Les journaux de transactions enregistrent le début et la fin de chaque transaction. Cela garantit que suffisamment d’informations est disponible au plus tard annuler ou restaurer des opérations dans la base de données.
  
Lorsque vous récupérez des erreurs dans lequel le fichier de base de données sur le disque est endommagé, mais les journaux de transaction sont intacts, votre application de restauration doit d’abord restaurer une bonne copie du fichier de base de données.
  
La banque d’informations Exchange relit les transactions de la transaction précédemment sauvegardée se connecte, puis relit les transactions restantes à partir des fichiers journaux des transactions sur le disque. Notez que parfois les transactions peuvent être perdues si le système échoue entre lorsque les transactions sont enregistrées dans les journaux de transactions et lorsqu’elles sont réellement écrites dans les fichiers de base de données. 
  
Périodiquement, la banque d’informations Exchange vérifie l’image de la base de données en mémoire, puis détermine les pages qui ont changé. La banque Exchange combine les modifications en attente, puis écrit ces pages dans le fichier de base de données sur le disque.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Fichiers de point de contrôle dans Exchange 2013

Enregistrements du fichier un point de contrôle qui a ouvert une session de transactions ont été écrits dans les fichiers de base de données sur le disque. Le point de contrôle est avancé lorsque toutes les pages qui ont été modifiés par des entrées de journaux de transactions de base de données sont correctement écrites sur le disque. Étant donné que le fichier de point de contrôle enregistre les transactions qui figurent déjà dans l’image de la base de données sur le disque, la banque d’informations Exchange ne doit relire les transactions effectuées après le point de contrôle. En fonction de la période de temps entre les sauvegardes, cela peut réduire considérablement le nombre de transactions qui doivent être relus dans la base de données en cas de défaillance du système.
  
## <a name="see-also"></a>Voir aussi

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    

