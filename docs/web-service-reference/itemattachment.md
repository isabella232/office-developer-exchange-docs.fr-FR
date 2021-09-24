---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: L’élément ItemAttachment représente un élément Exchange joint à un autre élément Exchange’élément.
ms.openlocfilehash: 09324e8f3cbd149cbe7cbd1a6291a703620e27fb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540881"
---
# <a name="itemattachment"></a>ItemAttachment

**L’élément ItemAttachment** représente un élément Exchange joint à un autre élément Exchange’élément. 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Message/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <CalendarItem/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Contact/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Task/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingMessage/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingRequest/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingResponse/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingCancellation/>
</ItemAttachment>
```

**ItemAttachmentType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifie la pièce jointe.  <br/> |
|[Name (AttachmentType)](name-attachmenttype.md) <br/> |Représente le nom de la pièce jointe.  <br/> |
|[ContentType](contenttype.md) <br/> |Décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe.  <br/> |
|[ContentId](contentid.md) <br/> |Représente un identificateur du contenu de la pièce jointe. [ContentId peut](contentid.md) être définie sur n’importe quelle valeur de chaîne. Les applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contient l’URI (Uniform Resource Identifier) qui correspond à l’emplacement du contenu de la pièce jointe.  <br/> |
|[Taille](size.md) <br/> |Représente la taille en octets de la pièce jointe du fichier.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Représente la dernière modification de la pièce jointe.  <br/> |
|[IsInline](isinline.md) <br/> |Représente si la pièce jointe apparaît en ligne dans un élément.  <br/> |
|[Élément](item.md) <br/> |Représente une pièce jointe générique Exchange’élément.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente une pièce jointe Exchange message électronique.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente une pièce jointe Exchange’élément de calendrier.  <br/> |
|[Contact](contact.md) <br/> |Représente une pièce jointe Exchange contact.  <br/> |
|[Tâche](task.md) <br/> |Représente une pièce jointe Exchange tâche.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Pièces jointes](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments et/ou fichiers joints à un élément dans la Exchange store.  <br/> |
   
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

