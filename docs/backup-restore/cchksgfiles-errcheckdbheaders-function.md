---
title: Fonction CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754752"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Fonction CChkSGFiles.ErrCheckDbHeaders

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valide les en-têtes des fichiers de base de données qui ont été spécifiés par la fonction **ErrInit** . Cette fonction renvoie également la taille de la page et le nombre de pages dans chacune des bases de données spécifiés. 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
Paramètre de sortie. La taille de page de chacune des bases de données spécifiées, en octets.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Paramètre de sortie. Le nombre de pages au début de chaque spécifié de base de données qui sont réservés par le moteur de base de données pour un usage interne. Notez que vous ne devez *pas* les pages d’en-tête passe à la fonction **ErrCheckDbPages** pour la validation. 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Paramètre de sortie. Si la valeur de retour de la fonction indique une erreur, ce paramètre est un index dans le tableau **[] rgwszDb** transmis à la fonction **ErrInit** . L’élément de tableau indexé représente la base de données dans laquelle l’erreur. Si la fonction ne retourne pas une valeur d’erreur, cette valeur de paramètre non valide. 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation future. La valeur passée doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoy�e

Cette fonction retourne un code d’erreur à partir de l' [énumération CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Remarques

**ErrCheckDbHeaders** vérifie que toutes les bases de données sont enregistrées avec **ErrInit** ont la même base de données et de signature page taille du journal. Vous pouvez également utiliser la valeur du paramètre **genMin** la plus faible et la valeur du paramètre **genMax** la plus élevée pour déterminer l’ensemble des fichiers journaux qui sont nécessaires pour mettre toutes les bases de données enregistrés à un état d’arrêt correct. 
  
Le paramètre **piDbErrorEncountered** est défini uniquement lorsqu’une erreur est détectée, comme indiqué par un zéro **ErrCheckDbHeaders** valeur de retour. 
  
Lorsqu’une erreur se produit dans cette fonction, un événement d’erreur sera ajouté au journal des événements Windows.
  
Vous pouvez appeler **ErrCheckDbHeaders** uniquement après l’appel de **ErrInit**, et vous devez l’appeler avant d’appeler **ErrCheckDbPages** et **ErrCheckLogs**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrCheckDbHeaders** dans la partie d’un seul thread, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

