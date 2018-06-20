---
title: Fonction CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Dernière modification : 03 mars 2013'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754744"
---
# <a name="cchksgfileserrinit-function"></a>Fonction CChkSGFiles.ErrInit
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Initialise l’objet **CChkSGFiles** en spécifiant les bases de données à vérifier et le chemin d’accès et nom de base des fichiers journaux des transactions à vérifier. Applications doivent appeler cette fonction immédiatement après l’appel avec succès la fonction **New** . 
  
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

### <a name="rgwszdb"></a>[] rgwszDb
  
Paramètre d’entrée. Tableau qui spécifie les bases de données à vérifier. Chaque élément de tableau est une chaîne Unicode terminée par le caractère null qui contient le chemin d’accès et le nom de base de données à vérifier.
    
### <a name="cdb"></a>cDB
  
Paramètre d’entrée. Le nombre d’éléments de chemin d’accès valide de la base de données dans le tableau **rgwszDb** . 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Paramètre d’entrée. Chemin d’accès complet des fichiers journaux des transactions à vérifier, sous la forme d’une chaîne Unicode terminée par null.
    
### <a name="wszbasename"></a>wszBaseName
  
Paramètre d’entrée. Le trois lettres nom de base les fichiers journaux des transactions, sous la forme d’une chaîne Unicode terminée par null.
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation future. La valeur transmise à ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoy�e

Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

La fonction **ErrInit** enregistre les bases de données et les fichiers journaux qui doivent être vérifiées. Cette fonction doit être appelée après la fonction **New** est appelée, mais avant toute autre **ChkSGFiles** l’appel de fonction. 
  
Vous devez fournir le nom de base, le chemin d’accès du fichier journal et tous les noms de base de données en tant que chaînes Unicode.
  
Vous pouvez vérifier que les fichiers de base de données, seuls les fichiers journaux ou les fichiers journaux et de base de données. Toutefois, lorsque vous appelez cette fonction, l’application doit spécifier au moins une entité à vérifier. Passer la valeur 0 (zéro) pour **cDB** et NULL pour **wszLogPath** renvoie une erreur. 
  
Si la valeur de **cDB** est différente de 0 (zéro), en passant NULL pour **rgwszDb** provoquera une erreur. Pour vérifier les fichiers de base de données, l’application doit fournir les noms de base de données. 
  
Si NULL est passé pour **wszBaseName** mais **wszLogPath** n’est pas NULL, une erreur sera renvoyée. Un nom de base du fichier journal est toujours requis lors de la vérification des fichiers journaux. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrInit** dans la partie d’un seul thread de l’application, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

