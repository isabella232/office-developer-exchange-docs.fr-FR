---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: L’élément WeeklyRecurrence décrit une périodicité hebdomadaire.
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530365"
---
# <a name="weeklyrecurrence"></a>WeeklyRecurrence

L’élément **WeeklyRecurrence** décrit une périodicité hebdomadaire. 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 **WeeklyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Interval](interval.md) <br/> |Définit l’intervalle, en semaines, entre deux éléments de modèle de périodicité hebdomadaire consécutifs. La valeur peut être comprise entre 1 et 99.  <br/> |
|[DaysOfWeek (DaysOfWeekType)](daysofweek-daysofweektype.md) <br/> |Décrit les jours de la semaine qui se trouvent dans le modèle de périodicité hebdomadaire.  <br/> |
|[FirstDayOfWeek](firstdayofweek.md) <br/> |Spécifie le premier jour de la semaine.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Périodicité (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
|[Récurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité des éléments de calendrier et des demandes de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de [fin](end-ex15websvcsotherref.md) de l’élément de gabarit périodique n’ont pas de date égale à la première occurrence d’une périodicité hebdomadaire. 
  
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

