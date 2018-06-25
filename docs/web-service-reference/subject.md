---
title: Objet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: c140d6c2-deb1-4f67-a908-9397197c4ae7
description: L’élément Subject représente la propriété subject d’éléments de banque Exchange. L’objet est limitée à 255 caractères.
ms.openlocfilehash: b93d64c6f517c1cc990d697061c8dad478eb3a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829612"
---
# <a name="subject"></a>Objet

L’élément **Subject** représente la propriété subject d’éléments de banque Exchange. L’objet est limitée à 255 caractères. 
  
```XML
<Subject/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente un objet de réponse Annuler calendrier élément.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Spécifie les critères pour les types de messages.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Représente un objet de réponse dynamique transfert des éléments.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion dans la banque d’informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique dans la banque d’informations Exchange.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
|[RemoveItem](removeitem.md) <br/> |Représente un objet de réponse d’élément remove.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Représente un objet de réponse dynamique répondre à tous.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Représente un objet de réponse dynamique à élément de réponse.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui contient l’objet d’un élément Exchange est requise.
  
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



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

