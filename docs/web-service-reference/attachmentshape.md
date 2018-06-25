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
description: L’élément AttachmentShape identifie des propriétés supplémentaires pour retourner une réponse à une demande GetAttachment.
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755339"
---
# <a name="attachmentshape"></a>AttachmentShape

L’élément **AttachmentShape** identifie des propriétés supplémentaires pour retourner une réponse à une demande [GetAttachment](getattachment.md) . 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse. Cet élément est facultatif.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifie la mise en forme le corps du texte dans la réponse. Cet élément est facultatif.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’une pièce jointe. Cet élément est facultatif.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires pour retourner une réponse. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |L’élément qui définit une demande pour obtenir une pièce jointe à partir d’une boîte aux lettres dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetAttachment](getattachment-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

