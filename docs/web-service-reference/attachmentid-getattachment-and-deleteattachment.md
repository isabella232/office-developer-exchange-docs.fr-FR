---
title: AttachmentId (GetAttachment et DeleteAttachment)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: L’élément AttachmentId identifie une seule pièce jointe.
ms.openlocfilehash: b0355b4a387c65e97fe973a1667e6b0a517ebf7e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755337"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a>AttachmentId (GetAttachment et DeleteAttachment)

L’élément **AttachmentId** identifie une seule pièce jointe. 
  
```xml
<AttachmentId Id="" />
```

 **RequestAttachmentIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Spécifie l’identificateur de pièce jointe.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentIds](attachmentids.md) <br/> | Contient un tableau d’identificateurs de pièce jointe.<br/><br/>  Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteAttachment](deleteattachment-operation.md)
- [Opération GetAttachment](getattachment-operation.md)

