---
title: ConversationIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationIndex
api_type:
- schema
ms.assetid: fdf47e22-8d93-4ae4-883b-0c9f07f48724
description: L’élément ConversationIndex contient un ID binaire qui représente le thread auquel appartient ce message.
ms.openlocfilehash: 5ca1c6cb27baa5ec1a2374c234103719ac952787
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526643"
---
# <a name="conversationindex"></a>ConversationIndex

**L’élément ConversationIndex** contient un ID binaire qui représente le thread auquel appartient ce message. 
  
```xml
<ConversationIndex/>
```

 **Base64Binary**
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
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente la réponse à une demande de réunion acceptée provisoirement.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contient un élément de la banque Exchange pour transférer à des destinataires.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente l'objet de réponse qui est utilisé pour annuler une réunion.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente un identificateur binaire au format **Base64Binary.** 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS du serveur Exchange sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

