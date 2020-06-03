---
title: Fonction fonction cchksgfiles. ErrCheckDbPages
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526724"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>Fonction fonction cchksgfiles. ErrCheckDbPages

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
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
  
Paramètre d’entrée. Index du tableau de bases de données spécifié dans le paramètre **rgwszDb []** de la fonction **ErrInit** . La base de données indexée par ce paramètre est vérifiée. 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
Paramètre d’entrée. Pointeur vers une mémoire tampon contenant une ou plusieurs pages de base de données à vérifier. La taille de la mémoire tampon doit être un multiple de la taille de la page de la base de données, tel qu’il est renvoyé dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** . L’application appelante doit remplir la mémoire tampon avec le contenu de la page de base de données avant d’appeler **ErrCheckDbPages**.
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
Paramètre d’entrée. Taille du paramètre **pvPageBuffer** , en octets. Cette valeur doit être un multiple de la taille de la page de la base de données, tel qu’il est renvoyé dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** . 
    
### <a name="rgpageinfo"></a>rgPageInfo[] 
  
Paramètre d’entrée/sortie. Tableau des structures **d' \_ infos sur la page** que **ErrCheckDbPages** remplit avec les résultats détaillés de chaque page de base de données qui est vérifiée. Le tableau doit avoir un élément pour chaque page de base de données passée dans le paramètre **pvPageBuffer** , et le champ **ulPgno** dans chaque structure d' ** \_ informations de page** doit être défini sur le numéro de page logique qui correspond à la page de base de données. Pour plus d’informations, consultez la section « Remarques » plus loin dans cette rubrique. 
    
### <a name="cpageinfo"></a>cPageInfo
  
Paramètre d’entrée. Nombre d’entrées dans le tableau **rgPageInfo []** . Cette valeur doit être égale au nombre de pages de base de données transmises dans le paramètre **pvPageBuffer** . 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée à un usage ultérieur. La valeur transmise dans ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

Notez que vous devez avoir spécifié la base de données dans le tableau de bases de données transmises à la fonction **ErrInit** . De plus, **ErrCheckDbHeaders** doit être appelé avant **ErrCheckDbPages**.
  
L’application appelante doit allouer un tampon de mémoire suffisamment grand pour contenir les pages de base de données à vérifier. L’application est chargée de remplir la mémoire tampon avec le contenu d’une ou de plusieurs pages de base de données de ce type. 
  
L’application appelante doit appeler **ErrCheckDbHeaders** avant d’appeler **ErrCheckDbPages**. Cette fonction peut être appelée autant de fois que nécessaire pour traiter toutes les pages de tous les fichiers de base de données qui doivent être vérifiés.
  
Dans le paramètre **rgPageInfo []** , chaque élément renvoyé contient des informations sur la page de base de données dans une structure d' ** \_ informations de page** . Si la fonction **ErrCheckDbPages** renvoie une erreur, l’application doit vérifier chaque structure d' ** \_ informations** pour déterminer la page sur laquelle l’erreur a été trouvée. Par exemple, la comparaison des valeurs **checksumActual** et **checksumExpected** indique si une erreur de checksum a été détectée sur cette page de base de données. 
  
Si **ErrCheckDbPages** détecte des erreurs dans le contenu de la base de données, il crée une entrée de journal d’événements d’erreurs Windows. 
  
L’objet **fonction cchksgfiles** détermine si toutes les bases de données enregistrées avec la fonction **ErrInit** ont été vérifiées. Plus précisément, **fonction cchksgfiles** utilise la fonction **ErrCheckDbPages** pour déterminer si le même nombre de pages de base de données indiqué par **ErrCheckDbHeaders** a été vérifié. Si le nombre correct de pages de chaque base de données n’a pas été correctement vérifié, la fonction **ErrTerm** renvoie une erreur. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckDbPages** dans la partie multithread de l’application. Notez que **ErrCheckDbPages** est généralement appelé plusieurs fois pour chaque base de données vérifiée. 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations de lecture pour la base de données et les fichiers journaux qui doivent être vérifiés.
  

