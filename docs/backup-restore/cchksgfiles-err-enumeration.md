---
title: Énumération CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: Dernière modification le 9 mars 2015
ms.openlocfilehash: 12cfff44a6dacbb07ee5518d0008092fbfb644d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510462"
---
# <a name="cchksgfileserr-enumeration"></a>Énumération CChkSGFiles.ERR 
  
**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Indique les résultats de la fonction appelée. Cette éumération est renvoyée par de nombreuses fonctions de la **classe CCheckSGFiles.** 
  
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
|errTaskDropped  <br/> |-106  <br/> |Renvoyé par la **fonction ErrTerm** pour indiquer que toutes les pages de base de données et les fichiers journaux des transactions n’ont pas été vérifiés ou que des erreurs ont été rencontrées pendant la vérification.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Un ou plusieurs fichiers journaux requis pour mettre la base de données à l’état d’arrêt sans interruption n’ont pas été trouvés dans le chemin d’accès du fichier journal ou n’ont pas le nom de base à trois lettres spécifié.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Un ou plusieurs paramètres transmis à la fonction n’étaient pas valides.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Une mémoire insuffisante était disponible pour terminer l’opération demandée.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |La sommes de contrôle stockée sur une page de base de données ne correspond pas à la sommes de contrôle attendue.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |La **fonction ErrTerm** a été appelée alors que l’objet était encore en cours d’utilisation. Cela peut se produire si **ErrTerm** est appelé avant le retour **d’ErrCheckDbPages** ou **d’ErrCheckLogFiles.**  <br/> |
   
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture sur la base de données et les fichiers journaux à vérifier.
  

