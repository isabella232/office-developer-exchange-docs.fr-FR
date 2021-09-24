---
title: Fonction CChkSGFiles.ErrCheckDbPages
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: e458e4ad552abfebb7611822a6e756bdd2ac6350
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510406"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>Fonction CChkSGFiles.ErrCheckDbPages

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valide une plage de pages dans une base de données spécifiée. 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="idb"></a>iDb
  
Paramètre d’entrée. Index dans le tableau de bases de données spécifié dans le paramètre **rgwszDb[]** de la **fonction ErrInit.** La base de données indexée par ce paramètre sera vérifiée. 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
Paramètre d’entrée. Pointeur vers une mémoire tampon contenant une ou plusieurs pages de base de données à vérifier. La taille de la mémoire tampon doit être un multiple de la taille de la page de base de données, comme renvoyé dans le paramètre **pcbDbPageSize** par la **fonction ErrCheckDbHeaders.** L’application appelant doit remplir la mémoire tampon avec le contenu de la page de base de données avant d’appeler **ErrCheckDbPages.**
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
Paramètre d’entrée. Taille du paramètre **pvPageBuffer,** en octets. Cette valeur doit être un multiple de la taille de la page de base de données, comme renvoyé dans le paramètre **pcbDbPageSize** par la **fonction ErrCheckDbHeaders.** 
    
### <a name="rgpageinfo"></a>rgPageInfo[] 
  
Paramètre d’entrée/sortie. Tableau de structures **PAGE \_ INFO** que **ErrCheckDbPages** remplit avec les résultats détaillés de chaque page de base de données vérifiée. Le tableau doit avoir un élément pour chaque page de base de données transmise dans le paramètre **pvPageBuffer,** et le champ **ulPgno** dans chaque structure **PAGE \_ INFO** doit être définie sur le numéro de page logique qui correspond à la page de base de données. Pour plus d’informations, voir « Remarques » plus loin dans cette rubrique. 
    
### <a name="cpageinfo"></a>cPageInfo
  
Paramètre d’entrée. Nombre d’entrées dans le **tableau rgPageInfo[].** Cette valeur doit être égale au nombre de pages de base de données transmises dans le **paramètre pvPageBuffer.** 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation ultérieure. La valeur transmise dans ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur de [l’éumération ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Remarques

Notez que vous devez avoir spécifié la base de données dans le tableau des bases de données transmises à la **fonction ErrInit.** En outre, **ErrCheckDbHeaders doit** être appelé avant **ErrCheckDbPages**.
  
L’application appelant doit allouer une mémoire tampon suffisamment grande pour contenir les pages de base de données à vérifier. L’application est responsable du remplissage de la mémoire tampon avec le contenu d’une ou de plusieurs pages de base de données de ce type. 
  
L’application appelant doit appeler **ErrCheckDbHeaders avant** **d’appeler ErrCheckDbPages.** Cette fonction peut être appelée autant de fois que nécessaire pour couvrir toutes les pages de tous les fichiers de base de données à vérifier.
  
Dans le **paramètre rgPageInfo[],** chaque élément renvoyé contient des informations sur la page de base de données dans une structure **PAGE \_ INFO.** Si la **fonction ErrCheckDbPages renvoie** une erreur, l’application doit vérifier chaque structure **PAGE \_ INFO** pour déterminer sur quelle page l’erreur a été trouvée. Par exemple, la comparaison des valeurs **checksumActual** et **checksumExpected** indique si une erreur de reprise de contrôle a été détectée sur cette page de base de données. 
  
Si **ErrCheckDbPages** détecte des erreurs dans le contenu de la base de données, il crée une entrée Windows journal des événements Error. 
  
**L’objet CChkSGFiles** détermine si toutes les bases de données enregistrées avec la fonction **ErrInit** ont été vérifiées. Plus précisément, **CChkSGFiles** utilise la fonction **ErrCheckDbPages** pour déterminer si le même nombre de pages de base de données indiqué par **ErrCheckDbHeaders** a été réellement vérifié. Si le nombre correct de pages dans chaque base de données n’a pas été correctement vérifié, la **fonction ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckDbPages** dans la partie multithread de l’application. Notez **que ErrCheckDbPages est** généralement appelé plusieurs fois pour chaque base de données vérifiée. 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations de lecture sur la base de données et les fichiers journaux qui doivent être vérifiés.
  

