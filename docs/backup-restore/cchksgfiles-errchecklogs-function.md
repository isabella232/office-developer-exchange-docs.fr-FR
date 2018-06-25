---
title: Fonction CChkSGFiles.ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754748"
---
# <a name="cchksgfileserrchecklogs-function"></a>Fonction CChkSGFiles.ErrCheckLogs

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valide les fichiers journaux de tous les fichiers de base de données n’a été spécifiés dans la fonction **ErrInit** . Les journaux validés sont ceux qui existent dans le chemin d’accès, et dont le nom de fichier journal de base de trois lettres transmis à **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Paramètre de sortie. Lorsque **la valeur true**, ce paramètre indique que les erreurs ont été trouvées dans les fichiers journaux des transactions, mais ces erreurs ont été tous trouvés dans les fichiers journaux qui ne sont pas nécessaires pour mettre la base de données à un état d’arrêt correct sans perte de données. Une valeur **true** est renvoyée dans ce paramètre est valide uniquement lorsque **ErrCheckLogs** renvoie **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation future. La valeur transmise à ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoy�e

Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) . 
  
Il est important de noter que cette fonction peut renvoyer **errSuccess** même cas d’erreurs dans les fichiers journaux. Par conséquent, lorsque **ErrCheckLogs** renvoie **errSuccess**, l’application doit également vérifier le paramètre de retour **pfOnlyUnnecessaryLogsCorrupt** . Si **pfOnlyUnnecessaryLogsCorrupts** a la **valeur true** lorsque **ErrCheckLogs** renvoie **errSuccess**, cela indique qu’une ou plusieurs erreurs ont été détectés, mais uniquement dans les fichiers journaux non nécessaires pour mettre à jour la base de données.
  
## <a name="remarks"></a>Remarques

La fonction **ErrCheckDbHeaders** doit être appelée avant que la fonction **ErrCheckLogs** peut être appelée. 
  
Lorsque les fichiers journaux des transactions de base de données sont vérifiées, certaines des fichiers journaux seront nécessaires pour mettre les bases de données dans le groupe de stockage pour un état d’arrêt correct sans perte de données, tandis que d’autres fichiers journaux ne peuvent pas être nécessaires. La fonction **ErrCheckLogs** détermine les plus anciens et les fichiers journaux plus récents qui sont nécessaires pour mettre à jour les bases de données. 
  
La fonction **ErrCheckLogs** vérifie tous les fichiers journaux dans les chemins d’accès spécifiés qui ont également le nom de fichier de base de trois lettres spécifié, tel qu’il est transmis à la fonction **ErrInit** . 
  
Si aucune erreur n’est détectée dans les fichiers journaux, **ErrCheckLogs** renvoie **errSuccess**. 
  
Si les fichiers journaux requis sont endommagées, **ErrCheckLogs** renvoie une erreur. 
  
Si des erreurs sont détectées uniquement dans les fichiers journaux qui sont antérieurs à la plus ancienne ceux qui sont nécessaires, la fonction renvoie **errSuccess** et définit le paramètre de retour **pfOnlyUnnecessaryLogCorrupt** sur **true**. L’application doit reconnaître qu’il existe des erreurs dans certains de ces fichiers journaux ancienne, et dans ce cas, il sera peut-être avertir l’utilisateur. Dans tous les cas, ces erreurs ne doivent pas affecter l’intégrité globale de la base de données ou affecter la réussite de lire les journaux.
  
Si des erreurs sont détectées dans tous les fichiers journaux créés après la plus proche journal détermine **ErrCheckLogs** est nécessaire, la fonction renvoie une erreur. L’erreur s’afficheront même si l’erreur du fichier journal a été trouvée dans un fichier journal qui a été généré postérieure à ce qui est nécessaire pour mettre à jour la base de données. Bien qu’il est possible de mettre les bases de données à un état d’arrêt correct à l’aide de fichiers journaux identifiés, spécifiées dans les fichiers plus tard endommagé journaux des transactions n’est pas appliquées, entraînant une perte de données lors de la base de données est restaurée. 
  
L’objet **CChkSGFiles** détermine si tous les fichiers journaux enregistrés avec la fonction **ErrInit** vérifiés réellement. Si ce n’est pas le cas, tous les journaux ont été correctement désactivée, la fonction **ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckLogs** dans la partie de l’application multithread, mais vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

