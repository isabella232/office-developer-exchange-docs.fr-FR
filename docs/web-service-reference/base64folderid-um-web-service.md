---
title: base64FolderId (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: L’élément base64FolderId contient l’identificateur du dossier pour spécifier que le dossier de courrier électronique par défaut à partir de laquelle la messagerie unifiée lit les messages par téléphone dans une requête (service web de messagerie unifiée) d’opération SetTelephoneAccessFolderEmail.
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755372"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (service web de messagerie unifiée)

L’élément **base64FolderId** contient l’identificateur du dossier pour spécifier que le dossier de courrier électronique par défaut à partir de laquelle la messagerie unifiée lit les messages par téléphone dans une requête [d’opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md) . 
  
[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (service web de messagerie unifiée)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Définit la demande pour définir le dossier de courrier électronique de l’accès téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de text représente l’ID MAPI du dossier.
  
## <a name="remarks"></a>Remarques

Pour définir le dossier de messages électroniques d’accès téléphonique, utilisez l' [opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Opération FindFolder](findfolder-operation.md)
  
[Opération FindItem](finditem-operation.md)

