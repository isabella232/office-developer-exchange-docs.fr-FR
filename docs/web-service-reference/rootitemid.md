---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: L’élément RootItemId identifie l’élément racine d’une pièce jointe supprimée.
ms.openlocfilehash: d8badd465fd5a93e1a6354d55ac5c4b080897152
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457094"
---
# <a name="rootitemid"></a>RootItemId

L’élément **RootItemId** identifie l’élément racine d’une pièce jointe supprimée. 
  
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
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande DeleteAttachment.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **RootItemId** est utilisé uniquement dans les réponses DeleteAttachment. Cela identifie l’identificateur de l’élément racine et, plus important, la nouvelle clé de modification de l’élément parent. 
  
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

