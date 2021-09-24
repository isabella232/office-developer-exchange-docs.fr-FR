---
title: ConversationTopic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationTopic
api_type:
- schema
ms.assetid: 46cacf42-4039-4c8a-9b20-c42cdd9f2760
description: L’élément ConversationTopic représente la rubrique de conversation.
ms.openlocfilehash: 38b208b957d36a2b0c876b33ef5c64a443b2f393
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529209"
---
# <a name="conversationtopic"></a>ConversationTopic

**L’élément ConversationTopic** représente la rubrique de conversation. 
  
```xml
<ConversationTopic/>
```

 **String**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Représente une réponse à accepter à une demande de réunion.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente un provisoire répond à une demande de réunion.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contient un élément de la banque Exchange pour transférer à des destinataires.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente l'objet de réponse qui est utilisé pour annuler une réunion.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente la rubrique du thread de conversation.
  
## <a name="remarks"></a>Remarques

La rubrique de conversation est généralement l’objet du premier message électronique d’un thread.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

