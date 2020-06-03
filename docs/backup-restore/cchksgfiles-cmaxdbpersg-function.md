---
title: Fonction fonction cchksgfiles. CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455260"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Fonction fonction cchksgfiles. CMaxDbPerSG

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le nombre maximal de bases de données autorisées dans un seul groupe de stockage Exchange Server.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Nombre maximal de bases de données que le serveur Exchange Server spécifié autorise par groupe de stockage. Étant donné que les groupes de stockage ne font pas partie d’Exchange 2013, cette fonction renvoie la valeur 1.
  
## <a name="remarks"></a>Remarques

Vous pouvez utiliser l’objet **CCheckSGFiles** pour valider des bases de données (et des fichiers journaux de transactions) dans un seul groupe de stockage, afin que la valeur renvoyée par la fonction **CMaxDbPerSG** représente également le nombre maximal de bases de données que vous pouvez vérifier à l’aide d’une instance de la classe **CCheckSGFiles** . 
  
Notez que, par défaut, Exchange Server 2003 et Exchange Server 2007 autorisent un maximum de cinq bases de données par groupe de stockage.
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

