---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: L’élément FileAttachment représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756368"
---
# <a name="fileattachment"></a>FileAttachment

L’élément **FileAttachment** représente un fichier qui est attaché à un élément dans la banque d’informations Exchange. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifie la pièce jointe.  <br/> |
|[Nom (AttachmentType)](name-attachmenttype.md) <br/> |Représente le nom de la pièce jointe.  <br/> |
|[ContentType](contenttype.md) <br/> |Décrit le type Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.  <br/> |
|[ContentId](contentid.md) <br/> |Représente un identificateur pour le contenu d’une pièce jointe. [ContentId](contentid.md) peut être définie à n’importe quelle valeur de chaîne. Applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contient l’identificateur de ressource uniforme (URI) qui correspond à l’emplacement du contenu de la pièce jointe.  <br/> |
|[Size](size.md) <br/> |Représente la taille en octets de la pièce jointe.  <br/> |
|[Heure de dernière modification](lastmodifiedtime.md) <br/> |Représente la dernière modification de la pièce jointe.  <br/> |
|[IsInline](isinline.md) <br/> |Indique si la pièce jointe apparaît en ligne au sein d’un élément.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Indique si la pièce jointe est une image du contact.  <br/> |
|[Content](content.md) <br/> |Contient le contenu de la pièce jointe codée en Base64.  <br/> |
   
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

