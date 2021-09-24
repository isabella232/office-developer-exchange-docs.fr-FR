---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: L’élément RelativeYearlyRecurrence décrit un modèle de périodité annuel relatif.
ms.openlocfilehash: ce6d724735cb23fb08bf541123341ede35011c4c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512498"
---
# <a name="relativeyearlyrecurrence"></a>RelativeYearlyRecurrence

**L’élément RelativeYearlyRecurrence** décrit un modèle de périodité annuel relatif. 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 **RelativeYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |Décrit les jours de la semaine qui sont utilisés dans les modèles de récurrence d’élément.  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |Décrit la semaine d’un mois utilisée dans une récurrence relative de l’année.  <br/> |
|[Month (périodicité d’élément)](month-item-recurrence.md) <br/> |Décrit le mois où se produit un élément périodique annuel.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la tendance de récurrence des éléments de calendrier et des demandes de réunion.  <br/> |
|[Standard](standard.md) <br/> |Représente la date et l’heure de passage de l’heure d’été à l’heure standard.  <br/> |
|[Daylight](daylight.md) <br/> |Représente la date et l’heure de passage de l’heure standard à l’heure d’été.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

