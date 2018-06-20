---
title: Fonction CChkSGFiles.New
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754740"
---
# <a name="cchksgfilesnew-function"></a>Fonction CChkSGFiles.New

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Crée une nouvelle instance de la classe **CChkSGFiles** . Vous devez appeler cette fonction avant de pouvoir spécifier le groupe de stockage et les bases de données à vérifier. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Référence (pointeur) à l’objet nouvellement créé.
  
## <a name="remarks"></a>Remarques

La fonction **New** crée un objet **CCheckSGFiles** et renvoie à l’appelant une référence (pointeur) à cet objet. Vous devez appeler cette fonction avant d’appeler toute autre fonction dans la classe **CCheckSGFiles** . 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **New** dans la partie d’un seul thread de l’application, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

