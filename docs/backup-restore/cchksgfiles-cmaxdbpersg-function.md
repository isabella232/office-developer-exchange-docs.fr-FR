---
title: Fonction CChkSGFiles.CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 1a82e71afde4766734d0875f68d7932a9fd9f26a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510524"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Fonction CChkSGFiles.CMaxDbPerSG

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Renvoie le nombre maximal de bases de données autorisées dans un groupe de stockage Exchange serveur unique.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Nombre maximal de bases de données que le serveur Exchange permet par groupe de stockage. Étant donné que les groupes de stockage ne font pas Exchange 2013, cette fonction renvoie 1.
  
## <a name="remarks"></a>Remarques

Vous pouvez utiliser l’objet **CCheckSGFiles** pour valider les bases de données (et les fichiers journaux des transactions) dans un seul groupe de stockage. La valeur renvoyée par la fonction **CMaxDbPerSG** représente également le nombre maximal de bases de données que vous pouvez vérifier à l’aide d’une instance de la classe **CCheckSGFiles.** 
  
Notez que par défaut, Exchange Server 2003 et Exchange Server 2007 autorisent un maximum de cinq bases de données par groupe de stockage.
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

