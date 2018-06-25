---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: L’élément IsRecurring indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique. Cet élément est en lecture seule.
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828104"
---
# <a name="isrecurring"></a>IsRecurring

L’élément **IsRecurring** indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique. Cet élément est en lecture seule. 
  
```xml
<IsRecurring/>
```

 **Boolean**
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
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise.
  
## <a name="remarks"></a>Remarques

Le tableau suivant montre comment la propriété **IsRecurring** est définie pour les types d’éléments de calendrier différent pour les organisateurs et les participants et pour les demandes de réunion et mises à jour. 
  
|**Type de CalendarItem**|**Organisateur <br/> (IsRecurring)**|**Attendee <br/> (IsRecurring)**|**Demande/mise à jour de réunion <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Occurrence unique  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|Périodique principal  <br/> |**FALSE** <br/> |**LA VALEUR TRUE** <br/> |**LA VALEUR TRUE** <br/> |
|Exception périodique  <br/> |**LA VALEUR TRUE** <br/> |**LA VALEUR TRUE** <br/> |**LA VALEUR TRUE** <br/> |
   
La valeur de la propriété **IsRecurring** qui est définie pour les éléments périodiques du calendrier principal pour l’organisateur est incorrecte ; Cette valeur doit être définie sur **TRUE**. 
  
> [!NOTE]
> L’opération GetUserAvailability a également un élément [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[TaskType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

