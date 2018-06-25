---
title: Fonction CChkSGFiles.Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754746"
---
# <a name="cchksgfilesdelete-function"></a>Fonction CChkSGFiles.Delete

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Détruit une instance existante de la classe **CChkSGFiles** . Vous devez appeler cette fonction après que l’application a terminé l’utilisation de l’objet spécifié. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Paramètres

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Paramètre d’entrée. Pointeur vers un objet **CCheckSGFiles** existant. La mémoire associée à l’objet puis sera libérée. 
    
## <a name="return-value"></a>Valeur renvoyée

Aucun.
  
## <a name="remarks"></a>Remarques

La fonction **Supprimer** libère la mémoire associée à l’objet **CCheckSGFiles** . Une fois que vous appelez **Delete**, le pointeur passé dans le paramètre *pcchecksgfiles* n’est pas valide et aucune autre opération ne peut être effectuées sur cet objet. 
  
Si l’application utilise la fonction **ErrCheckDbPages** , l’application doit libérer la mémoire tampon manuellement. la fonction **Supprimer** sera libère pas. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **Supprimer** dans la partie d’un seul thread de l’application, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

