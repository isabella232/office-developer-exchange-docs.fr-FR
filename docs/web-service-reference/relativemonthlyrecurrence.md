---
title: RelativeMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: L’élément RelativeMonthlyRecurrence décrit une périodité mensuelle relative.
ms.openlocfilehash: 326e6581e55e64ffd2bcc9bdfa5108cf63089633
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513443"
---
# <a name="relativemonthlyrecurrence"></a>RelativeMonthlyRecurrence

**L’élément RelativeMonthlyRecurrence** décrit une périodité mensuelle relative. 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 **RelativeMonthlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Interval](interval.md) <br/> |Définit l’intervalle entre deux éléments périodiques mensuels consécutifs. La plage de cette valeur est de 1 à 99.  <br/> |
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |Décrit les jours de la semaine dans la récurrence mensuelle relative.  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |Décrit la semaine utilisée dans une récurrence mensuelle relative.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la tendance de récurrence des éléments de calendrier et des demandes de réunion.  <br/> |
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
   
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

