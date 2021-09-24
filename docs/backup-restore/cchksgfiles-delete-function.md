---
title: Fonction CChkSGFiles.Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: cf1c23dd75442d73dfea49e0831d0859da321a40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510539"
---
# <a name="cchksgfilesdelete-function"></a>Fonction CChkSGFiles.Delete

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Détruit une instance existante de la **classe CChkSGFiles.** Vous devez appeler cette fonction une fois que l’application a terminé de travailler avec l’objet spécifié. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Paramètres

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Paramètre d’entrée. Pointeur vers un objet **CCheckSGFiles** existant. La mémoire associée à l’objet est ensuite libérée. 
    
## <a name="return-value"></a>Valeur renvoyée

Aucun.
  
## <a name="remarks"></a>Remarques

La **fonction Delete** libère la mémoire associée à l’objet **CCheckSGFiles.** Après avoir appelé **Delete,** le pointeur transmis dans le paramètre  *pcchecksgfiles*  n’est pas valide et aucune autre opération ne peut être effectuée sur cet objet. 
  
Si l’application utilise **la fonction ErrCheckDbPages,** l’application doit libérer la mémoire tampon manuellement . la **fonction Delete** ne la libère pas. 
  
Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **Delete** dans la partie monothread de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles.** 
  
## <a name="requirements"></a>Configuration requise

Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

