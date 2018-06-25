---
title: SetTelephoneAccessFolderEmail (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: L’élément SetTelephoneAccessFolderEmail définit une demande pour définir le dossier par défaut des messages électroniques à partir de laquelle la messagerie unifiée sera lire des messages par téléphone.
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a>SetTelephoneAccessFolderEmail (service web de messagerie unifiée)

L’élément **SetTelephoneAccessFolderEmail** définit une demande pour définir le dossier par défaut des messages électroniques à partir de laquelle la messagerie unifiée sera lire des messages par téléphone. 
  
[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[base64FolderId (service web de messagerie unifiée)](base64folderid-um-web-service.md) <br/> |L’identificateur du dossier de courrier électronique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md)

