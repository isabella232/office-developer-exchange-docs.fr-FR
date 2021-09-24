---
title: Fonction CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Last modified: March 03, 2013'
ms.openlocfilehash: ccb5293e35f20328181c4cf1cb5f0eddbb42e03f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516292"
---
# <a name="cchksgfileserrinit-function"></a>Fonction CChkSGFiles.ErrInit
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Initialise l’objet **CChkSGFiles** en spécifiant les bases de données à vérifier et le chemin d’accès et le nom de base des fichiers journaux des transactions à vérifier. Les applications doivent appeler cette fonction immédiatement après l’appel réussi **de la fonction New.** 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="rgwszdb"></a>rgwszDb[]
  
Paramètre d’entrée. Tableau qui spécifie les bases de données à vérifier. Chaque élément de tableau est une chaîne Unicode terminée par null qui contient le chemin d’accès et le nom de fichier d’une base de données à vérifier.
    
### <a name="cdb"></a>cDB
  
Paramètre d’entrée. Nombre d’éléments de chemin de base de données valides dans le tableau **rgwszDb.** 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Paramètre d’entrée. Chemin d’accès complet des fichiers journaux des transactions à vérifier, sous la forme d’une chaîne Unicode terminée par null.
    
### <a name="wszbasename"></a>wszBaseName
  
Paramètre d’entrée. Nom de base à trois lettres du Exchange journaux des transactions, sous la forme d’une chaîne Unicode terminée par null.
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation ultérieure. La valeur transmise par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur de [l’éumération ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Remarques

La **fonction ErrInit** enregistre les bases de données et les fichiers journaux à vérifier. Cette fonction doit être appelée après l’appel de la fonction **New,** mais avant toute autre fonction **ChkSGFiles.** 
  
Vous devez fournir tous les noms de base de données, le chemin d’accès au fichier journal et le nom de base en tant que chaînes Unicode terminées par null.
  
Vous pouvez vérifier uniquement les fichiers de base de données, uniquement les fichiers journaux, ou les fichiers de base de données et les fichiers journaux. Toutefois, lors de l’appel de cette fonction, l’application doit spécifier au moins une entité à vérifier. La transmission de 0 (zéro)  **pour cDB**  et NULL pour  **wszLogPath**  retourne une erreur. 
  
Si la valeur de  **cDB**  est autre que 0 (zéro), la transmission de null pour  **rgwszDb**  entraîne une erreur. Pour vérifier les fichiers de base de données, l’application doit fournir les noms de base de données. 
  
Si NULL est transmis pour  **wszBaseName**  mais  **que wszLogPath**  n’est pas NULL, une erreur est renvoyée. Un nom de base de fichier journal est toujours requis lors de la vérification des fichiers journaux. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrInit** dans la partie monothread de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

