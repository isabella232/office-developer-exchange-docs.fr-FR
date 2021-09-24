---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: L’élément RootItemId identifie l’élément racine d’une pièce jointe supprimée.
ms.openlocfilehash: eab3cc30c2e3f2b6cdc443ba8eb7ae4bfa38d257
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509366"
---
# <a name="rootitemid"></a>RootItemId

**L’élément RootItemId** identifie l’élément racine d’une pièce jointe supprimée. 
  
[DeleteAttachmentResponse](deleteattachmentresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
  
[RootItemId](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **RootItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**RootItemId** <br/> |Identifie l’élément racine d’une pièce jointe supprimée.  <br/> |
|**RootItemChangeKey** <br/> |Identifie la nouvelle clé de modification de l’élément racine d’une pièce jointe supprimée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande DeleteAttachment.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément RootItemId** est utilisé uniquement dans les réponses DeleteAttachment. Cela permet d’identifier l’identificateur de l’élément racine et, plus important encore, la nouvelle clé de modification de l’élément parent. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[DeleteAttachment](deleteattachment.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

