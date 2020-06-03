---
title: Fonction cchksgfiles. ERR, énumération
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
description: Dernière modification le 9 mars 2015
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455253"
---
# <a name="cchksgfileserr-enumeration"></a>Fonction cchksgfiles. ERR, énumération 
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Indique les résultats de la fonction appelée. Cette énumération est renvoyée par de nombreuses fonctions de la classe **CCheckSGFiles** . 
  
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

## <a name="values"></a>Values

|**Nom du membre**|**Valeur**|**Description**|
|:-----|:-----|:-----|
|errSuccess  <br/> |0  <br/> |La fonction s’est terminée sans erreur.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Renvoyé par la fonction **ErrTerm** pour indiquer que toutes les pages de base de données et tous les fichiers journaux de transaction ont été vérifiés, ou que des erreurs ont été rencontrées lors de la vérification.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Un ou plusieurs fichiers journaux requis pour ramener la base de données à un état d’arrêt correct n’ont pas été trouvés dans le chemin d’accès au fichier journal, ou n’ont pas le nom de base à trois lettres spécifié.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Un ou plusieurs paramètres transmis à la fonction ne sont pas valides.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Mémoire insuffisante pour terminer l’opération demandée.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |La somme de contrôle stockée sur une page de base de données ne correspond pas à son checksum attendu.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |La fonction **ErrTerm** a été appelée alors que l’objet était toujours en cours d’utilisation. Cela peut se produire si **ErrTerm** est appelé avant que **ErrCheckDbPages** ou **ErrCheckLogFiles** n’ait été renvoyé.  <br/> |
   
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

