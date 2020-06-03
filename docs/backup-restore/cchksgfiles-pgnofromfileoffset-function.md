---
title: Fonction fonction cchksgfiles. PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452894"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Fonction fonction cchksgfiles. PgnoFromFileOffset

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le numéro de page de base de données logique correspondant à l’index d’octet spécifié dans le fichier de base de données physique. Si le décalage du fichier n’est pas valide ou si la fonction **ErrCheckDbHeaders** n’a pas été appelée pour les bases de données, cette fonction renvoie la valeur 0 (zéro). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Paramètres

### <a name="ibfileoffset"></a>ibFileOffset
  
Paramètre d’entrée. Offset dans un fichier de base de données, en octets.
    
## <a name="return-value"></a>Valeur renvoyée

Numéro de page logique du fichier de base de données qui inclut le décalage spécifié.
  
## <a name="remarks"></a>Remarques

Si le paramètre **ibFileOffset** n’est pas valide, la fonction **PgnoFromFileOffset** renvoie 0 (zéro). 
  
**PgnoFromFileOffset** renvoie également 0 (zéro) si vous n’avez pas appelé la fonction **ErrCheckDbHeaders** sur l’instance **CCheckSGFiles** . Vous devez appeler **ErrCheckDbHeaders** pour initialiser la taille de la page de base de données et le nombre de pages allouées aux en-têtes de base de données. 
  
Vous devez utiliser **PgnoFromFileOffset** pour remplir les éléments de structure d' ** \_ informations** en préparation à l’appel de **ErrCheckDbPages**. Le paramètre **rgPageInfo** de **ErrCheckDbPages** exige que chaque élément du tableau soit une structure **PAGE_INFO** , avec les valeurs de membre **ulPgno** correctement initialisées. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **PgnoFromFileOffset** dans la partie multithread de l’application. Notez que vous appelez généralement cette fonction plusieurs fois pour chaque base de données vérifiée. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’une autorisation de lecture sur la base de données et les fichiers journaux à vérifier.
  

