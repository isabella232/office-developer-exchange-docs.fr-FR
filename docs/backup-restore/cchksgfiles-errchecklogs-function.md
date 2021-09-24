---
title: Fonction CChkSGFiles.ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 64484b32fdc566d6fee8631f80d078aca82b11d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516383"
---
# <a name="cchksgfileserrchecklogs-function"></a>Fonction CChkSGFiles.ErrCheckLogs

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valide les fichiers journaux de tous les fichiers de base de données qui ont été spécifiés dans la **fonction ErrInit.** Les journaux validés sont ceux qui existent dans le chemin d’accès et dont le nom de fichier journal de base à trois lettres est transmis à **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Paramètre de sortie. Lorsque la valeur est **true,** ce paramètre indique que des erreurs ont été trouvées dans les fichiers journaux de transactions, mais que ces erreurs ont toutes été trouvées dans les fichiers journaux qui ne sont pas nécessaires pour mettre la base de données à un état d’arrêt sans perte de données. Une **valeur true** renvoyée dans ce paramètre est valide uniquement lorsque **ErrCheckLogs** renvoie **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation ultérieure. La valeur transmise par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur de [l’éumération ERR.](cchksgfiles-err-enumeration.md) 
  
Il est important de se souvenir que cette fonction peut renvoyer **errSuccess** même lorsque des erreurs sont trouvées dans les fichiers journaux. Par conséquent, lorsque **ErrCheckLogs** renvoie **errSuccess,** l’application doit également vérifier le paramètre de retour **pfOnlyUnnecessaryLogsCorrupt.** Si **pfOnlyUnnecessaryLogsCorrupts** a la valeur **true** lorsque **ErrCheckLogs** renvoie **errSuccess,** cela indique qu’une ou plusieurs erreurs ont été trouvées, mais uniquement dans les fichiers journaux qui ne sont pas nécessaires pour mettre à jour la base de données.
  
## <a name="remarks"></a>Remarques

La **fonction ErrCheckDbHeaders doit** être appelée avant que la fonction **ErrCheckLogs** puisse être appelée. 
  
Lors de la vérification des fichiers journaux de transactions de la base de données Exchange, certains fichiers journaux sont nécessaires pour mettre les bases de données du groupe de stockage à un état d’arrêt sans perte de données, alors que d’autres fichiers journaux peuvent ne pas être nécessaires. La **fonction ErrCheckLogs** détermine les fichiers journaux les plus anciens et les plus récents nécessaires pour mettre à jour les bases de données. 
  
La **fonction ErrCheckLogs** vérifie tous les fichiers journaux dans les chemins d’accès spécifiés qui ont également le nom de fichier de base à trois lettres spécifié, tel qu’il est transmis à la fonction **ErrInit.** 
  
Si aucune erreur n’est trouvée dans les fichiers journaux, **ErrCheckLogs** renvoie **errSuccess**. 
  
Si l’un des fichiers journaux requis est endommagé, **ErrCheckLogs** renvoie une erreur. 
  
Si des erreurs sont trouvées uniquement dans les fichiers journaux plus anciens que les plus anciens nécessaires, la fonction renvoie **errSuccess** et définit le paramètre de retour **pfOnlyUnnecessaryLogCorrupt** sur **true**. L’application doit reconnaître qu’il existe des erreurs dans certains de ces anciens fichiers journaux, et si c’est le cas, elle peut alerter l’utilisateur. Dans tous les cas, ces erreurs ne doivent pas affecter l’intégrité globale de la base de données ou affecter la réussite de la lecture des journaux.
  
Si des erreurs sont trouvées dans un fichier journal créé après que le journal le plus tôt **qu’ErrCheckLogs** détermine est nécessaire, la fonction renvoie une erreur. L’erreur est renvoyée même si l’erreur du fichier journal a été trouvée dans un fichier journal qui a été généré plus tard que ce qui est nécessaire pour mettre à jour la base de données. Bien qu’il soit possible de mettre les bases de données à un état de nettoyage à l’aide des fichiers journaux identifiés, les transactions spécifiées dans les fichiers journaux endommagés ultérieurement ne sont pas appliquées, ce qui entraîne une perte de données lors de la restauration de la base de données. 
  
**L’objet CChkSGFiles** détermine si tous les fichiers journaux enregistrés avec la fonction **ErrInit** ont été réellement vérifiés. Si tous les journaux n’ont pas été correctement vérifiés, la **fonction ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckLogs** dans la partie multithread de l’application, mais vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture sur la base de données et les fichiers journaux à vérifier.
  

