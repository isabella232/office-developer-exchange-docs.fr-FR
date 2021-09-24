---
title: Fonction CChkSGFiles.ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Last modified: February 25, 2013'
ms.openlocfilehash: 152fd613ef461d8c1ef69401237cfea09cd32b08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516285"
---
# <a name="cchksgfileserrterm-function"></a>Fonction CChkSGFiles.ErrTerm
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fournit un état global de la vérification de la base de données et des journaux, qui indique si toutes les pages de base de données et tous les journaux ont été vérifiés avec succès.
  
> [!IMPORTANT]
> Stockage groupes ne sont pas disponibles dans Exchange 2013. Pour la compatibilité ascendante avec les bases de données et les groupes de stockage dans les versions de Exchange antérieures à Exchange Server 2010, l’API CHKSGFILES vous permet de spécifier des groupes de stockage. Lorsque vous exécutez CHKSGFILES sur des bases de données Exchange 2013, vous devez définir des paramètres qui spécifient un identificateur de groupe de stockage sur une chaîne vide. 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation ultérieure. La valeur transmise par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur de [l’éumération ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Remarques

**L’objet CChkSGFiles** détermine si toutes les bases de données enregistrées avec la fonction **ErrInit** ont été vérifiées. Cet objet utilise la **fonction ErrCheckDbPages** pour vérifier que le même nombre de pages de base de données identifié par la fonction **ErrCheckDbHeaders** a été réellement vérifié. Si le nombre correct de pages dans chaque base de données n’est pas correctement vérifié, la **fonction ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données vérifiées avec **ErrCheckDbPages** est inférieur à celui indiqué par **ErrCheckDbHeaders**, cette fonction crée une erreur dans le journal des événements Windows et **ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données vérifiées avec **ErrCheckDbPages** est supérieur à celui indiqué par **ErrCheckDbHeaders,** cette fonction crée un avertissement dans le journal des événements Windows pour indiquer que l’application peut vérifier inutilement certaines pages de base de données plusieurs fois. Dans ce cas, toutefois, la **fonction ErrTerm** réussit. 
  
**L’objet CChkSGFiles détermine** également si les fichiers journaux enregistrés avec **ErrInit** ont été réellement vérifiés. Si tous les journaux n’ont pas été correctement vérifiés, la **fonction ErrTerm** renvoie une erreur. 
  
Lorsque **ErrTerm** renvoie une erreur, il s’agit de la première erreur qu’il trouve, même s’il vérifie l’état de vérification de toutes les bases de données enregistrées avec **ErrInit**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrTerm** dans la partie monothread de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

