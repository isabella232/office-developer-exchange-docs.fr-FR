---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: L’élément FileAttachment représente un fichier joint à un élément dans la Exchange store.
ms.openlocfilehash: 66424fefafd2084bf0b6f45881089448593e621d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518497"
---
# <a name="fileattachment"></a>FileAttachment

**L’élément FileAttachment** représente un fichier joint à un élément dans la Exchange store. 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 **FileAttachmentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifie la pièce jointe du fichier.  <br/> |
|[Name (AttachmentType)](name-attachmenttype.md) <br/> |Représente le nom de la pièce jointe.  <br/> |
|[ContentType](contenttype.md) <br/> |Décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe.  <br/> |
|[ContentId](contentid.md) <br/> |Représente un identificateur pour le contenu d’une pièce jointe. [ContentId peut](contentid.md) être définie sur n’importe quelle valeur de chaîne. Les applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contient l’URI (Uniform Resource Identifier) qui correspond à l’emplacement du contenu de la pièce jointe.  <br/> |
|[Taille](size.md) <br/> |Représente la taille en octets de la pièce jointe du fichier.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Représente la dernière modification de la pièce jointe.  <br/> |
|[IsInline](isinline.md) <br/> |Représente si la pièce jointe apparaît en ligne dans un élément.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Indique si la pièce jointe du fichier est une image de contact.  <br/> |
|[Content](content.md) <br/> |Contient le contenu codé en Base64 de la pièce jointe du fichier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

