---
title: Fonction CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 3e2845cc326520ad875dc8bda52bac3d7c2e2cfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516243"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Fonction CChkSGFiles.PgnoFromFileOffset

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le numéro de page de base de données logique qui correspond à l’index d’byte spécifié dans le fichier de base de données physique. Si le décalage de fichier n’est pas valide ou si la fonction **ErrCheckDbHeaders** n’a pas été appelée pour les bases de données, cette fonction renvoie 0 (zéro). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Paramètres

### <a name="ibfileoffset"></a>fileOffset
  
Paramètre d’entrée. Décalage dans un fichier de base de données, en octets.
    
## <a name="return-value"></a>Valeur renvoyée

Numéro de page logique du fichier de base de données qui inclut le décalage spécifié.
  
## <a name="remarks"></a>Remarques

Si le **paramètrefileOffset** n’est pas valide, la **fonction PgnoFromFileOffset** renvoie 0 (zéro). 
  
**PgnoFromFileOffset** renvoie également 0 (zéro) si vous n’avez pas appelé la fonction **ErrCheckDbHeaders** sur l’instance **CCheckSGFiles.** Vous devez appeler **ErrCheckDbHeaders** pour initialiser la taille de la page de base de données et le nombre de pages allouées aux en-têtes de base de données. 
  
Vous devez utiliser **PgnoFromFileOffset** pour remplir les éléments de structure **PAGE \_ INFO** en préparation de l’appel **d’ErrCheckDbPages.** Le **paramètre rgPageInfo** vers **ErrCheckDbPages** nécessite que chaque élément du tableau soit une structure **PAGE_INFO,** avec les valeurs de membre **ulPgno** correctement initialisées. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **PgnoFromFileOffset** dans la partie multithread de l’application. Notez que vous appelez généralement cette fonction plusieurs fois pour chaque base de données en cours de vérification. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir une autorisation de lecture sur la base de données et les fichiers journaux qui doivent être vérifiés.
  

