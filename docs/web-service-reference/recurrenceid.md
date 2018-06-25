---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: L’élément RecurrenceId est utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829005"
---
# <a name="recurrenceid"></a>RecurrenceId

L’élément **RecurrenceId** est utilisé pour identifier une instance spécifique d’un élément de calendrier périodique. 
  
```xml
<RecurrenceId/>
```

 **dateTime**
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
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente une valeur de date/heure qui identifie une occurrence de calendrier.
  
## <a name="remarks"></a>Remarques

Cette propriété est utilisée avec la propriété [UID](uid.md) pour identifier une instance spécifique d’un élément de calendrier périodique. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

