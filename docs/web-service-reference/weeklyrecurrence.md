---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: L’élément WeeklyRecurrence décrit une périodité hebdomadaire.
ms.openlocfilehash: 408116dd85fb31fce8f5f3b5b4cde92945783f5d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509335"
---
# <a name="weeklyrecurrence"></a>WeeklyRecurrence

**L’élément WeeklyRecurrence** décrit une périodité hebdomadaire. 
  
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
|[Interval](interval.md) <br/> |Définit l’intervalle, en semaines, entre deux éléments de modèle de récurrence hebdomadaire consécutifs. La valeur peut être dans la plage de 1 à 99.  <br/> |
|[DaysOfWeek (DaysOfWeekType)](daysofweek-daysofweektype.md) <br/> |Décrit les jours de la semaine dans la récurrence hebdomadaire.  <br/> |
|[FirstDayOfWeek](firstdayofweek.md) <br/> |Spécifie le premier jour de la semaine.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la tendance de récurrence des éléments de calendrier et des demandes de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les informations de décalage de [](start.md) fuseau horaire sont perdues si les [dates](end-ex15websvcsotherref.md) de début et de fin de l’élément principal périodique ne sont pas égales à la première occurrence d’une fréquence hebdomadaire de récurrence. 
  
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

