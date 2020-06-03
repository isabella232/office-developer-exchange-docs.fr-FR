---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: L’élément ConversationId contient l’identificateur d’un élément ou d’une conversation.
ms.openlocfilehash: 4f12d70ae6b72773760a731f5778cf6743ce699f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461470"
---
# <a name="conversationid"></a>ConversationId

L’élément **ConversationId** contient l’identificateur d’un élément ou d’une conversation. 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Identifie un élément spécifique dans la Banque d’informations Exchange.  <br/> |
|**ChangeKey** <br/> | Identifie une version spécifique d’un élément. Un **ChangeKey** est requis pour les scénarios suivants :  <br/><br/>-L’élément [UpdateItem](updateitem.md) nécessite un **ChangeKey** si l’attribut **ConflictResolution** est défini sur autosolve. Autosolve est une valeur par défaut. Si l’attribut **ChangeKey** n’est pas inclus, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorChangeKeyRequired**.<br/><br/>- Les éléments [SendItem](senditem.md), [DeleteItem](deleteitem.md)et [DeleteFolder](deletefolder.md) requièrent un **ChangeKey** pour tester si l’opération tentée agira sur la version la plus récente d’un élément. Si l’attribut **ChangeKey** n’est pas inclus dans l' **ItemId** ou si **ChangeKey** est vide, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[ConversationAction](conversationaction.md) <br/> |Représente une action unique à appliquer à une conversation unique.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément post dans la Banque d’Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
   
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

- [Opération FindConversation](findconversation-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

