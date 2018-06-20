---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: L’élément RelativeYearlyRecurrence décrit une périodicité annuelle relative.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829057"
---
# <a name="relativeyearlyrecurrence"></a>RelativeYearlyRecurrence

L’élément **RelativeYearlyRecurrence** décrit une périodicité annuelle relative. 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 **RelativeYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |Décrit les jours de la semaine qui sont utilisés dans l’élément périodicités.  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |Décrit la semaine du mois est utilisée dans une périodicité annuelle relative.  <br/> |
|[Mois (élément périodicité)](month-item-recurrence.md) <br/> |Décrit le mois quand un élément périodique annuel se produit.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Périodicité (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de périodicité pour les tâches répétitives.  <br/> |
|[Périodicité (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité pour les éléments de calendrier et les demandes de réunion.  <br/> |
|[Standard](standard.md) <br/> |Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.  <br/> |
|[Heure d’été](daylight.md) <br/> |Représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

