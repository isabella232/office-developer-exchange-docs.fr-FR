---
title: Périodicité (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: L’élément de périodicité contient la périodicité pour les éléments de calendrier et les demandes de réunion.
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829004"
---
# <a name="recurrence-recurrencetype"></a>Périodicité (RecurrenceType)

L’élément de **périodicité** contient la périodicité pour les éléments de calendrier et les demandes de réunion. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 **RecurrenceType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une périodicité annuelle relative.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Représente une périodicité annuelle.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit une périodicité mensuelle relative d’un élément de calendrier périodique.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Représente une périodicité mensuelle.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit la fréquence, en semaines, ainsi que les jours un élément de calendrier ou une tâche est périodique.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Décrit la fréquence, en jours, dans laquelle un élément de calendrier ou une tâche est périodique.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Décrit une périodicité qui n’a pas une date de fin définie.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Décrit la date de début et date de fin de périodicité d’un élément.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Décrit la date de début et le nombre d’occurrences d’un élément périodique.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d’informations Exchange  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster. 
  
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

