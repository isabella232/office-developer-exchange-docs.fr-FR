---
title: Fonction fonction cchksgfiles. Delete
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447049"
---
# <a name="cchksgfilesdelete-function"></a>Fonction fonction cchksgfiles. Delete

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Détruit une instance existante de la classe **fonction cchksgfiles** . Vous devez appeler cette fonction une fois que l’application a fini de travailler avec l’objet spécifié. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Paramètres

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Paramètre d’entrée. Pointeur vers un objet **CCheckSGFiles** existant. La mémoire associée à l’objet sera ensuite libérée. 
    
## <a name="return-value"></a>Valeur renvoyée

Aucun.
  
## <a name="remarks"></a>Remarques

La fonction **Delete** libère la mémoire associée à l’objet **CCheckSGFiles** . Une fois que vous avez appelé **Delete**, le pointeur transmis dans le paramètre *pcchecksgfiles* n’est pas valide et aucune autre opération ne peut être effectuée sur cet objet. 
  
Si l’application utilise la fonction **ErrCheckDbPages** , l’application doit libérer la mémoire tampon manuellement ; la fonction **Delete** ne la libère pas. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **Delete** dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** . 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

