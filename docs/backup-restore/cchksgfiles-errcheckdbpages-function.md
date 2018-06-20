---
title: Fonction CChkSGFiles.ErrCheckDbPages
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754745"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>Fonction CChkSGFiles.ErrCheckDbPages

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Valide une plage de pages dans une base de données spécifié. 
  
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
  
Paramètre d’entrée. Un index dans le tableau des bases de données spécifié dans le paramètre **[] rgwszDb** à la fonction **ErrInit** . La base de données indexée par ce paramètre sera vérifiée. 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
Paramètre d’entrée. Pointeur vers un tampon qui contient une ou plusieurs pages de base de données à vérifier. La taille de la mémoire tampon doit être un multiple de la taille de page de base de données, renvoyée dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** . L’application appelante doit remplir la mémoire tampon avec le contenu de page de base de données avant d’appeler **ErrCheckDbPages**.
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
Paramètre d’entrée. La taille du paramètre **pvPageBuffer** , en octets. Cette valeur doit être un multiple de la taille de page de base de données, renvoyée dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** . 
    
### <a name="rgpageinfo"></a>[] rgPageInfo 
  
Paramètre d’entrée/sortie. Un tableau de **PAGE\_INFO** structures **ErrCheckDbPages** remplit avec le détail des résultats de chaque page de base de données est vérifiée. Le tableau doit avoir un élément pour chaque page de base de données transmis dans le paramètre **pvPageBuffer** et le champ **ulPgno** dans chaque **PAGE\_INFO** structure doit être définie sur le numéro de page logique qui correspond à la page de base de données. Pour plus d’informations, voir « Remarques » plus loin dans cette rubrique. 
    
### <a name="cpageinfo"></a>cPageInfo
  
Paramètre d’entrée. Le nombre d’entrées dans le tableau **[] rgPageInfo** . Cette valeur doit être égale au nombre de pages de base de données transmis dans le paramètre **pvPageBuffer** . 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation future. La valeur passée dans ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoy�e

Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

Notez que vous devez avoir spécifié la base de données dans le tableau des bases de données transmis à la fonction **ErrInit** . En outre, **ErrCheckDbHeaders** doit être appelé avant **ErrCheckDbPages**.
  
L’application appelante doit allouer une mémoire tampon qui est suffisante pour contenir les pages de base de données à vérifier. L’application est chargée pour remplir la mémoire tampon avec le contenu d’une ou plusieurs des pages de base de données. 
  
L’application appelante doit appeler **ErrCheckDbHeaders** avant d’appeler **ErrCheckDbPages**. Cette fonction peut être appelée autant de fois que nécessaire pour couvrir toutes les pages de tous les fichiers de base de données qui doivent être vérifiées.
  
Dans le paramètre **[] rgPageInfo** , chaque élément renvoyé contient des informations sur la page de base de données dans un **PAGE\_INFO** structure. Si la fonction **ErrCheckDbPages** renvoie une erreur, l’application doit vérifier chacune **PAGE\_INFO** structure pour déterminer la page sur laquelle l’erreur a été trouvé. Par exemple, comparant les valeurs **checksumActual** et **checksumExpected** indique si une erreur de somme de contrôle a été détectée sur cette page de la base de données. 
  
Si **ErrCheckDbPages** détecte des erreurs dans le contenu de la base de données, il crée une entrée de journal des événements d’erreur Windows. 
  
L’objet **CChkSGFiles** détermine si les bases de données qui utilisent la fonction **ErrInit** ont été réellement activés. Plus précisément, **CChkSGFiles** utilise la fonction de **ErrCheckDbPages** pour déterminer si le même nombre de pages de base de données indiqué par **ErrCheckDbHeaders** ont été vérifié réellement. Si le nombre approprié de pages dans chaque base de données n’ont pas été archivé avec succès, la fonction **ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckDbPages** dans la partie de l’application multithread. Notez que **ErrCheckDbPages** est généralement appelée plusieurs fois pour chaque base de données est vérifiée. 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit avoir lecture des autorisations pour les fichiers journaux et de base de données qui doivent être vérifiées.
  

