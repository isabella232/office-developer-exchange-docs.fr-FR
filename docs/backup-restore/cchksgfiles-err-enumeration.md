---
title: Énumération CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: 'Derni�re modification�: lundi 9 mars 2015'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755691"
---
# <a name="cchksgfileserr-enumeration"></a>Énumération CChkSGFiles.ERR 
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Indique le résultat de la fonction appelée. Cette énumération est retournée par de nombreuses fonctions de la classe **CCheckSGFiles** . 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a>Valeurs

|**Nom du membre**|**Valeur**|**Description**|
|:-----|:-----|:-----|
|errSuccess  <br/> |0  <br/> |La fonction s’est terminée sans erreur.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Renvoyée par la fonction **ErrTerm** pour indiquer que pas toutes les pages de base de données et fichiers journaux des transactions ont été vérifiées, ou que des erreurs se sont produites pendant la vérification.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Un ou plusieurs fichiers journaux qui sont nécessaires pour faire de la base de données à un état d’arrêt correct est introuvable dans le chemin d’accès du fichier journal, ou n’a pas le nom de base de trois lettres spécifié.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Un ou plusieurs paramètres qui ont été transmis à la fonction ne sont pas valides.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Mémoire insuffisante n’était disponible pour effectuer l’opération demandée.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |La somme de contrôle qui est stocké dans une page de base de données ne correspond pas à la somme de contrôle attendue.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |La fonction **ErrTerm** a été appelée alors que l’objet a été en cours d’utilisation. Cela peut se produire si **ErrTerm** est appelé avant **ErrCheckDbPages** ou **ErrCheckLogFiles** a renvoyé.  <br/> |
   
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

