---
title: Fonction CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: e50b41e761b8e46d778011b6bac3db4dbb624809
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516271"
---
# <a name="cchksgfilesnew-function"></a>Fonction CChkSGFiles.New

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Crée une instance de la **classe CChkSGFiles.** Vous devez appeler cette fonction avant de pouvoir spécifier le groupe de stockage et les bases de données à vérifier. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Paramètres

Aucun.
  
## <a name="return-value"></a>Valeur renvoyée

Référence (pointeur) à l’objet nouvellement créé.
  
## <a name="remarks"></a>Remarques

La **fonction New** crée un objet **CCheckSGFiles** et renvoie à l’appelant une référence (pointeur) à cet objet. Vous devez appeler cette fonction avant d’appeler l’une des autres fonctions de la classe **CCheckSGFiles.** 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **New** dans la partie monothread de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

