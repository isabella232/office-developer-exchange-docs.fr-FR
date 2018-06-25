---
title: Pièces jointes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: L’élément de pièces jointes contient les éléments ou les fichiers associés à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: 8aa5c0849122f5ca83485459fce5d0fea449c974
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755340"
---
# <a name="attachments"></a>Pièces jointes

L’élément de **pièces jointes** contient les éléments ou les fichiers associés à un élément dans la banque d’informations Exchange. 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 **ArrayOfAttachmentsType** et **NonEmptyArrayOfAttachmentsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Définit une demande pour créer une pièce jointe à un élément dans la banque d’informations Exchange.<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/CreateAttachment` <br/> |
|[AcceptItem](acceptitem.md) <br/> | Représente une réponse à accepter à une demande de réunion.<br/><br/>Voici quelques-unes des expressions XPath pour cet élément :<ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente un provisoire répond à une demande de réunion.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Item](item.md) <br/> |Représente un élément Exchange générique.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande GetAttachment.  <br/> |
   
## <a name="remarks"></a>Remarques

Les éléments de **pièces jointes** ont les mêmes éléments enfants mais sont basées sur différents types : **ArrayOfAttachmentsType** et **NonEmptyArrayOfAttachmentsType**. Les types de définissent si un élément enfant est nécessaire. **ArrayOfAttachmentsType** est utilisé uniquement dans le message de réponse. Il est également important de noter que ces éléments se produisent dans les messages et les types d’espaces de noms. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

