---
title: Fonction CChkSGFiles.ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Dernière modification : 25 février 2013'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754750"
---
# <a name="cchksgfileserrterm-function"></a>Fonction CChkSGFiles.ErrTerm
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fournit un état global de la vérification de base de données et journaux, ce qui indique si les pages de base de données et les journaux ont été vérifiées avec succès.
  
> [!IMPORTANT]
> Groupes de stockage ne sont pas disponibles dans Exchange 2013. Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange Server 2010, l’API CHKSGFILES vous permet de spécifier les groupes de stockage. Lorsque vous exécutez CHKSGFILES par rapport à des bases de données Exchange 2013, vous devez définir les paramètres que vous spécifiez un identificateur de groupe de stockage sur une chaîne vide. 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée pour une utilisation future. La valeur transmise à ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoy�e

Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

L’objet **CChkSGFiles** détermine si les bases de données qui utilisent la fonction **ErrInit** ont été réellement activés. Cet objet utilise la fonction **ErrCheckDbPages** pour vérifier que le même nombre de pages identifiées par la fonction **ErrCheckDbHeaders** ont été vérifiées réellement de base de données. Si le nombre approprié de pages dans chaque base de données n’est pas vérifié avec succès, la fonction **ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données avec **ErrCheckDbPages** est inférieur à celui indiqué par **ErrCheckDbHeaders**, cette fonction crée une erreur dans le journal des événements Windows et **ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données avec **ErrCheckDbPages** est supérieur à celle indiquée par **ErrCheckDbHeaders**, cette fonction crée un message d’avertissement dans le journal des événements Windows pour indiquer que l’application peut inutilement contrôler certains pages de base de données plusieurs fois. Dans ce cas, toutefois, la fonction **ErrTerm** réussit. 
  
L’objet **CChkSGFiles** détermine également si les fichiers journaux enregistrés avec **ErrInit** vérifiés réellement. Si ce n’est pas le cas, tous les journaux ont été correctement activé, la fonction **ErrTerm** renvoie une erreur. 
  
Lorsque **ErrTerm** renvoie une erreur, il sera la première erreur qu’il trouve, même si elle vérifie l’état de vérification pour toutes les bases de données sont enregistrées avec **ErrInit**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrTerm** dans la partie d’un seul thread de l’application, et vous ne pouvez l’appeler aucuns plus qu’une fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

