---
title: base64FolderId (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: L’élément base64FolderId contient l’identificateur du dossier à spécifier comme dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lit les messages par téléphone dans une demande d’opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée).
ms.openlocfilehash: 149ad55d0ab09f57b0dc3ace7eb0e17c96265e3f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518931"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (service web de messagerie unifiée)

L’élément **base64FolderId** contient l’identificateur du dossier à spécifier comme dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lit les messages par téléphone dans une demande d’opération [SetTelephoneAccessFolderEmail (service web](settelephoneaccessfolderemail-operation-um-web-service.md) de messagerie unifiée). 
  
[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (service web de messagerie unifiée)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Définit la demande de définition du dossier de messagerie d’accès téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte représente l’ID MAPI du dossier.
  
## <a name="remarks"></a>Remarques

Pour définir le dossier de messagerie d’accès téléphonique, utilisez l’opération [SetTelephoneAccessFolderEmail (service web de messagerie unie).](settelephoneaccessfolderemail-operation-um-web-service.md)
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Opération FindFolder](findfolder-operation.md)
  
[Opération FindItem](finditem-operation.md)

