---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: L’élément ItemAttachment représente un élément Exchange qui est attaché à un autre élément Exchange.
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828137"
---
# <a name="itemattachment"></a>ItemAttachment

L’élément **ItemAttachment** représente un élément Exchange qui est attaché à un autre élément Exchange. 
  
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

 **ItemAttachmentType**
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
|[ContentId](contentid.md) <br/> |Représente un identificateur pour le contenu de la pièce jointe. [ContentId](contentid.md) peut être définie à n’importe quelle valeur de chaîne. Applications peuvent utiliser [ContentId](contentid.md) pour implémenter leurs propres mécanismes d’identification.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contient l’identificateur de ressource uniforme (URI) qui correspond à l’emplacement du contenu de la pièce jointe.  <br/> |
|[Size](size.md) <br/> |Représente la taille en octets de la pièce jointe.  <br/> |
|[Heure de dernière modification](lastmodifiedtime.md) <br/> |Représente la dernière modification de la pièce jointe.  <br/> |
|[IsInline](isinline.md) <br/> |Indique si la pièce jointe apparaît en ligne au sein d’un élément.  <br/> |
|[Item](item.md) <br/> |Représente une pièce jointe d’élément Exchange générique.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente une pièce jointe du message électronique Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente une pièce jointe élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente les pièces jointes à un élément de contact d’Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une pièce jointe de tâche Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Pièces jointes](attachments-ex15websvcsotherref.md) <br/> |Contient les articles et/ou les fichiers associés à un élément dans la banque d’informations Exchange.  <br/> |
   
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

