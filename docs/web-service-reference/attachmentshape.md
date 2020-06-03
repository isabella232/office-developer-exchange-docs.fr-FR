---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: L’élément AttachmentShape identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529664"
---
# <a name="attachmentshape"></a>AttachmentShape

L’élément **AttachmentShape** identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) . 
  
- [GetAttachment](getattachment.md)
  
- [AttachmentShape](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 **AttachmentResponseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |Indique si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse. Cet élément est facultatif.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifie la façon dont le corps de texte est mis en forme dans la réponse. Cet élément est facultatif.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Indique si le contenu HTML potentiellement dangereux est filtré à partir d’une pièce jointe. Cet élément est facultatif.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires à renvoyer dans une réponse. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |Élément qui définit une demande d’obtention d’une pièce jointe à partir d’une boîte aux lettres dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetAttachment](getattachment-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

