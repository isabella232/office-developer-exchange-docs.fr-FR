---
title: Fonction CChkSGFiles.CMaxDbPerSG
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755708"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Fonction CChkSGFiles.CMaxDbPerSG

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le nombre maximal de bases de données autorisées dans un seul groupe de stockage de serveur Exchange.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Le nombre maximal de bases de données qui permet du serveur Exchange spécifié par le groupe de stockage. Étant donné que les groupes de stockage ne font pas partie d’Exchange 2013, cette fonction renvoie 1.
  
## <a name="remarks"></a>Remarques

Vous pouvez utiliser l’objet **CCheckSGFiles** pour valider des bases de données (et les fichiers journaux des transactions) qu’un seul groupe de stockage, de sorte que la valeur renvoyée par la fonction **CMaxDbPerSG** représente également le nombre maximal de bases de données que vous pouvez le vérifier en utilisant un instance de la classe **CCheckSGFiles** . 
  
Notez que par défaut, Exchange Server 2003 et Exchange Server 2007 autorisent un maximum de cinq bases de données par groupe de stockage.
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

