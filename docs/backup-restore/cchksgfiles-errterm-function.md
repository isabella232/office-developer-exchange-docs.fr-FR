---
title: Fonction fonction cchksgfiles. ErrTerm
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
ms.openlocfilehash: 12b07fba69054d327c7250bbf83e4c77016e8b3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466198"
---
# <a name="cchksgfileserrterm-function"></a>Fonction fonction cchksgfiles. ErrTerm
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fournit un état global de la vérification de la base de données et du journal, qui indique si toutes les pages de base de données et les journaux ont été vérifiés.
  
> [!IMPORTANT]
> Les groupes de stockage ne sont pas disponibles dans Exchange 2013. Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange Server 2010, l’API CHKSGFILES vous permet de spécifier des groupes de stockage. Lorsque vous exécutez CHKSGFILES sur des bases de données Exchange 2013, vous devez définir des paramètres qui spécifient un identificateur de groupe de stockage sur une chaîne vide. 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Paramètres

### <a name="ulflags"></a>ulFlags
  
Paramètre d’entrée facultatif. Cette valeur est réservée à un usage ultérieur. La valeur passée par ce paramètre doit être 0 (zéro).
    
## <a name="return-value"></a>Valeur renvoyée

Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Remarques

L’objet **fonction cchksgfiles** détermine si toutes les bases de données enregistrées avec la fonction **ErrInit** ont été vérifiées. Cet objet utilise la fonction **ErrCheckDbPages** pour vérifier que le même nombre de pages de base de données identifiées par la fonction **ErrCheckDbHeaders** ont été vérifiées. Si le nombre correct de pages de chaque base de données n’est pas correctement vérifié, la fonction **ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données vérifiées avec **ErrCheckDbPages** est inférieur à celui indiqué par **ErrCheckDbHeaders**, cette fonction génère une erreur dans le journal des événements Windows et **ErrTerm** renvoie une erreur. 
  
Si le nombre de pages de base de données vérifiées avec **ErrCheckDbPages** est supérieur à celui indiqué par **ErrCheckDbHeaders**, cette fonction crée un avertissement dans le journal des événements Windows pour indiquer que l’application peut ne pas vérifier plusieurs fois certaines pages de base de données. Dans ce cas, toutefois, la fonction **ErrTerm** réussit. 
  
L’objet **fonction cchksgfiles** détermine également si les fichiers journaux enregistrés avec **ErrInit** ont été vérifiés. Si tous les journaux n’ont pas été correctement vérifiés, la fonction **ErrTerm** renvoie une erreur. 
  
Lorsque **ErrTerm** renvoie une erreur, il s’agit de la première erreur trouvée, même si elle vérifie l’état de vérification de toutes les bases de données inscrites avec **ErrInit**.
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrTerm** dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

