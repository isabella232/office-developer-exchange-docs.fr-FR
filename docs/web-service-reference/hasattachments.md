---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: L'élément HasAttachments représente une propriété qui est définie sur true si un élément a au moins un des pièces jointes visible ou si une conversation contient au moins un élément qui comporte une pièce jointe. Cette propriété est en lecture seule.
ms.openlocfilehash: cc4e4ec0eac1c749723facc8cd780da41b0d8150
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462921"
---
# <a name="hasattachments"></a>HasAttachments

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **HasAttachments** représente une propriété qui est définie sur **true** si un élément a au moins un des pièces jointes visible ou si une conversation contient au moins un élément qui comporte une pièce jointe. Cette propriété est en lecture seule. 
  
```XML
<HasAttachments/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Conditions](conditions.md) <br/> |Représente les conditions qui, une fois traité, déclenche les actions de règle associée à cette règle.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Exceptions](exceptions.md) <br/> |Représente toutes les conditions d'exception de règle disponibles pour la règle de boîte de réception.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur Boolean est requise. La valeur **true** signifie que l'élément ou la conversation a au moins un des pièces jointes visible. La valeur **false** signifie que la conversation ou un élément n'a aucune pièce jointe ou a masqué uniquement les pièces jointes. 
  
## <a name="remarks"></a>Remarques

La propriété **HasAttachments** est calculée à partir de la propriété MAPI booléenne **AllAttachmentsHidden**. Si un élément n'a pas de pièce jointe, la propriété **AllAttachmentsHidden** n'existe pas. Si toutes les pièces jointes sur l'élément sont masqués, la propriété **AllAttachmentsHidden** est **true**. La propriété **AllAttachmentsHidden** est **false** si elle a au moins une pièce jointe et au moins une des pièces jointes est visible. Utilisez la propriété MAPI **AllAttachmentsHidden** pour la recherche, de regroupement et de tri des éléments. 
  
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
  
[Référence EWS pour Exchange](ews-reference-for-exchange.md)

