---
title: Fonction CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 215a0d1126fce48b7e3800016619b0c52915312b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510469"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Fonction CChkSGFiles.ErrCheckDbHeaders

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Valide les en-têtes des fichiers de base de données spécifiés par la **fonction ErrInit.** Cette fonction renvoie également la taille de page et le nombre de pages dans chacune des bases de données spécifiées. 
  
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
  
Paramètre de sortie. Nombre de pages au début de chaque base de données spécifiée qui sont réservées par le moteur de base de données pour une utilisation interne. Notez que vous ne *devez pas* transmettre de pages d’en-tête à la **fonction ErrCheckDbPages** pour validation. 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Paramètre de sortie. Si la valeur de retour de la fonction indique une erreur, ce paramètre sera un index dans le tableau **rgwszDb[]** transmis à la **fonction ErrInit.** L’élément de tableau indexé représente la base de données dans laquelle l’erreur s’est produite. Si la fonction ne retourne pas de valeur d’erreur, cette valeur de paramètre n’est pas valide. 
    
### <a name="ulflags"></a>ulFlags 
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation ultérieure. La valeur transmise doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Cette fonction renvoie un code d’erreur à partir de [l’éumération CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Remarques

**ErrCheckDbHeaders** vérifie que toutes les bases de données inscrites auprès **d’ErrInit** ont la même signature de journal et la même taille de page de base de données. Vous pouvez également utiliser la valeur de paramètre **genMin** la plus faible et la valeur de paramètre **genMax** la plus élevée pour déterminer l’ensemble des fichiers journaux nécessaires pour mettre toutes les bases de données enregistrées à un état d’arrêt sans nettoyage. 
  
Le **paramètre piDbErrorEncountered** est définie uniquement lorsqu’une erreur est détectée, comme indiqué par une valeur de retour **ErrCheckDbHeaders** non nulle. 
  
Lorsqu’une erreur se produit dans cette fonction, un événement d’erreur est ajouté au journal Windows événements Error.
  
Vous pouvez appeler **ErrCheckDbHeaders** uniquement après avoir appelé **ErrInit** et vous devez l’appeler avant d’appeler **ErrCheckDbPages** et **ErrCheckLogs**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrCheckDbHeaders** dans la partie monothread et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture sur la base de données et les fichiers journaux à vérifier.
  

