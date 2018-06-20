---
title: Fonction CChkSGFiles.PgnoFromFileOffset
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754753"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Fonction CChkSGFiles.PgnoFromFileOffset

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le numéro de page logique de la base de données qui correspond à l’index spécifié d’octets dans le fichier de base de données physique. Si le décalage de fichier n’est pas valide, ou si la fonction **ErrCheckDbHeaders** n’a pas été appelée pour les bases de données, cette fonction renvoie la valeur 0 (zéro). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Paramètres

### <a name="ibfileoffset"></a>ibFileOffset
  
Paramètre d’entrée. Offset dans un fichier de base de données, en octets.
    
## <a name="return-value"></a>Valeur renvoy�e

Numéro de page logique du fichier de base de données qui inclut l’offset spécifié.
  
## <a name="remarks"></a>Remarques

Si le paramètre **ibFileOffset** n’est pas valide, la fonction **PgnoFromFileOffset** renvoie la valeur 0 (zéro). 
  
**PgnoFromFileOffset** renvoie également 0 (zéro) si vous n’avez pas appelé la fonction **ErrCheckDbHeaders** sur l’instance **CCheckSGFiles** . Vous devez appeler **ErrCheckDbHeaders** pour initialiser la taille de page de base de données et du nombre de pages allouées aux en-têtes de base de données. 
  
Vous devez utiliser **PgnoFromFileOffset** pour remplir le **PAGE\_INFO** éléments en vue de l’appel **ErrCheckDbPages**de structure. Le paramètre **rgPageInfo** pour **ErrCheckDbPages** requiert une structure **PAGE_INFO** , avec les valeurs du membre **ulPgno** correctement initialisé chaque élément dans le tableau. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **PgnoFromFileOffset** dans la partie de l’application multithread. Notez que vous devez généralement appeler cette fonction plusieurs fois pour chaque base de données en cours d’archivage. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
L’application s’exécute sous le compte doit avoir autorisation de lecture sur les base de données et les fichiers journaux qui doivent être vérifiées.
  

