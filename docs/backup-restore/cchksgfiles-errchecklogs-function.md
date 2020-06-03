---
title: Fonction fonction cchksgfiles. ErrCheckLogs
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 71e21bb3a748a532f9e3167e0b36898acde71b02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526717"
---
# <a name="cchksgfileserrchecklogs-function"></a>Fonction fonction cchksgfiles. ErrCheckLogs

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valide les fichiers journaux de tous les fichiers de base de données qui ont été spécifiés dans la fonction **ErrInit** . Les journaux validés sont ceux qui existent dans le chemin d’accès et dont le nom de fichier journal de base à trois lettres est transmis à **ErrInit**.
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
Paramètre de sortie. Lorsque la **valeur est true**, ce paramètre indique que des erreurs ont été détectées dans les fichiers journaux des transactions, mais ces erreurs se sont produites dans les fichiers journaux qui ne sont pas nécessaires pour amener la base de données à un état d’arrêt correct sans perte de données. Une valeur **true** renvoyée dans ce paramètre est valide uniquement lorsque **ErrCheckLogs** renvoie **errSuccess**. 
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée à un usage ultérieur. La valeur passée par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) . 
  
N’oubliez pas que cette fonction peut renvoyer **errSuccess** même si des erreurs sont détectées dans les fichiers journaux. Par conséquent, lorsque **ErrCheckLogs** renvoie **errSuccess**, l’application doit également vérifier le paramètre de retour **pfOnlyUnnecessaryLogsCorrupt** . Si **pfOnlyUnnecessaryLogsCorrupts** a la **valeur true** lorsque **ErrCheckLogs** renvoie **errSuccess**, cela indique qu’une ou plusieurs erreurs ont été détectées, mais uniquement dans les fichiers journaux qui n’ont pas besoin de mettre à jour la base de données.
  
## <a name="remarks"></a>Remarques

La fonction **ErrCheckDbHeaders** doit être appelée avant que la fonction **ErrCheckLogs** puisse être appelée. 
  
Lorsque les fichiers journaux de transaction de base de données Exchange sont vérifiés, certains fichiers journaux sont nécessaires pour mettre les bases de données dans le groupe de stockage à un état d’arrêt correct sans perte de données, tandis que d’autres fichiers journaux peuvent ne pas être nécessaires. La fonction **ErrCheckLogs** détermine les fichiers journaux les plus anciens et les plus récents nécessaires pour mettre à jour les bases de données. 
  
La fonction **ErrCheckLogs** vérifie tous les fichiers journaux dans les chemins d’accès spécifiés qui ont également le nom de fichier de base à trois lettres spécifié, comme transmis à la fonction **ErrInit** . 
  
Si aucune erreur n’est détectée dans les fichiers journaux, **ErrCheckLogs** renvoie **errSuccess**. 
  
Si l’un des fichiers journaux requis est endommagé, **ErrCheckLogs** renvoie une erreur. 
  
Si des erreurs sont détectées uniquement dans les fichiers journaux plus anciens que ceux nécessaires, la fonction renvoie **errSuccess** et définit le paramètre de retour **pfOnlyUnnecessaryLogCorrupt** sur **true**. L’application doit reconnaître qu’il existe des erreurs dans certains de ces anciens fichiers journaux et, si tel est le cas, elle peut alerter l’utilisateur. Dans tous les cas, ces erreurs ne doivent pas influer sur l’intégrité globale de la base de données ou sur la réussite ou l’échec de la lecture des journaux.
  
Si des erreurs sont détectées dans un fichier journal créé après le premier journal déterminé par **ErrCheckLogs** , la fonction renvoie une erreur. L’erreur est renvoyée même si l’erreur du fichier journal a été trouvée dans un fichier journal généré plus tard que ce qui est nécessaire pour mettre à jour la base de données. Bien qu’il soit possible de ramener les bases de données à un état d’arrêt correct à l’aide des fichiers journaux identifiés, les transactions spécifiées dans les fichiers journaux endommagés les plus récents ne sont pas appliquées, ce qui entraîne une perte de données lors de la restauration de la base de données. 
  
L’objet **fonction cchksgfiles** détermine si tous les fichiers journaux enregistrés avec la fonction **ErrInit** ont été vérifiés. Si tous les journaux n’ont pas été correctement vérifiés, la fonction **ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckLogs** dans la partie multithread de l’application, mais vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

