---
title: Fonction fonction cchksgfiles. ErrCheckDbHeaders
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455246"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Fonction fonction cchksgfiles. ErrCheckDbHeaders

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valide les en-têtes des fichiers de base de données qui ont été spécifiés par la fonction **ErrInit** . Cette fonction renvoie également la taille de la page et le nombre de pages dans chacune des bases de données spécifiées. 
  
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
  
Paramètre de sortie. Taille de page de chacune des bases de données spécifiées, en octets.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Paramètre de sortie. Nombre de pages au début de chaque base de données spécifiée qui sont réservées par le moteur de base de données à des fins d’utilisation interne. Notez que vous ne devez *pas* transmettre de pages d’en-tête à la fonction **ErrCheckDbPages** pour la validation. 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Paramètre de sortie. Si la valeur renvoyée par la fonction indique une erreur, ce paramètre correspond à un index dans le tableau **rgwszDb []** passé à la fonction **ErrInit** . L’élément de tableau indexé représente la base de données dans laquelle l’erreur a été rencontrée. Si la fonction ne renvoie pas de valeur d’erreur, la valeur de ce paramètre n’est pas valide. 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée à un usage ultérieur. La valeur transmise doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Cette fonction renvoie un code d’erreur à partir de l' [énumération fonction cchksgfiles. err](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Remarques

**ErrCheckDbHeaders** vérifie que toutes les bases de données enregistrées avec **ErrInit** ont la même signature de journal et la même taille de page de base de données. Vous pouvez également utiliser la valeur de paramètre **genMin** la plus faible et la valeur du paramètre **genMax** la plus élevée pour déterminer le jeu de fichiers journaux nécessaires pour mettre toutes les bases de données enregistrées à un état d’arrêt correct. 
  
Le paramètre **piDbErrorEncountered** est défini uniquement lorsqu’une erreur est détectée, comme indiqué par une valeur de retour différente de zéro **ErrCheckDbHeaders** . 
  
Lorsqu’une erreur se produit dans cette fonction, un événement d’erreur est ajouté au journal des événements d’erreurs de Windows.
  
Vous ne pouvez appeler **ErrCheckDbHeaders** qu’après avoir appelé **ErrInit**, et vous devez l’appeler avant d’appeler **ErrCheckDbPages** et **ErrCheckLogs**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrCheckDbHeaders** dans la partie à thread unique, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

