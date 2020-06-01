---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: L’élément DailyRecurrence décrit la fréquence, en jours, à laquelle un élément de calendrier ou une tâche se répète.
ms.openlocfilehash: d18a04ced19c87996c3a092f6668ab00c5a3f006
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462170"
---
# <a name="dailyrecurrence"></a>DailyRecurrence

L’élément **DailyRecurrence** décrit la fréquence, en jours, à laquelle un élément de calendrier ou une tâche se répète. 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

**DailyRecurrencePatternType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Interval](interval.md) <br/> |Définit l’intervalle, en jours, entre deux éléments périodiques consécutifs. La valeur doit être comprise entre 1 et 999.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Périodicité (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
|[Récurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité des éléments de calendrier et des demandes de réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

