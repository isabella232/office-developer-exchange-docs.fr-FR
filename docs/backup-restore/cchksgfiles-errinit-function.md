---
title: Fonction fonction cchksgfiles. ErrInit
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
description: 'Dernière modification : 1er mars 2013'
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457010"
---
# <a name="cchksgfileserrinit-function"></a>Fonction fonction cchksgfiles. ErrInit
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Initialise l’objet **fonction cchksgfiles** en spécifiant les bases de données à vérifier et le chemin d’accès et le nom de base des fichiers journaux de transactions à vérifier. Les applications doivent appeler cette fonction immédiatement après avoir réussi à appeler la **nouvelle** fonction. 
  
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
  
Paramètre d’entrée. Tableau qui spécifie les bases de données à vérifier. Chaque élément de tableau est une chaîne Unicode terminée par un caractère null qui contient le chemin d’accès et le nom de fichier d’une base de données à vérifier.
    
### <a name="cdb"></a>cDB
  
Paramètre d’entrée. Nombre d’éléments de chemin d’accès de base de données valides dans le tableau **rgwszDb** . 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Paramètre d’entrée. Chemin d’accès complet des fichiers du journal des transactions à vérifier, sous la forme d’une chaîne Unicode terminée par un caractère null.
    
### <a name="wszbasename"></a>wszBaseName
  
Paramètre d’entrée. Nom de base à trois lettres des fichiers journaux de transactions Exchange, sous la forme d’une chaîne Unicode terminée par un caractère null.
    
### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée à un usage ultérieur. La valeur passée par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

La fonction **ErrInit** enregistre les bases de données et les fichiers journaux qui doivent être vérifiés. Cette fonction doit être appelée après l’appel de la fonction **New** , mais avant l’appel de toute autre fonction **ChkSGFiles** . 
  
Vous devez fournir tous les noms de base de données, le chemin d’accès au fichier journal et le nom de base comme chaînes Unicode terminées par un caractère null.
  
Vous pouvez vérifier uniquement les fichiers de base de données, uniquement les fichiers journaux, ou les fichiers de base de données et les fichiers journaux. Toutefois, lors de l’appel de cette fonction, l’application doit spécifier au moins une entité à vérifier. Le passage de la valeur 0 (zéro) pour **CDB** et null pour **wszLogPath** renvoie une erreur. 
  
Si la valeur de **CDB** est différente de 0 (zéro), le fait de transmettre null pour **rgwszDb** génère une erreur. Pour vérifier les fichiers de base de données, l’application doit fournir les noms de base de données. 
  
Si NULL est passé pour **wszBaseName** mais **wszLogPath** n’est pas null, une erreur est renvoyée. Un nom de base de fichier journal est toujours requis lors de la vérification des fichiers journaux. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrInit** dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

