---
title: Fonction fonction cchksgfiles. New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455232"
---
# <a name="cchksgfilesnew-function"></a>Fonction fonction cchksgfiles. New

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Crée une instance de la classe **fonction cchksgfiles** . Vous devez appeler cette fonction pour pouvoir spécifier le groupe de stockage et les bases de données à vérifier. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Référence (pointeur) à l’objet nouvellement créé.
  
## <a name="remarks"></a>Remarques

La **nouvelle** fonction crée un objet **CCheckSGFiles** et renvoie à l’appelant une référence (pointeur) à cet objet. Vous devez appeler cette fonction avant d’appeler une des autres fonctions de la classe **CCheckSGFiles** . 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la **nouvelle** fonction dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

