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
description: L’élément DailyRecurrence décrit la fréquence, en jours, dans laquelle un élément de calendrier ou d’une tâche est périodique.
ms.openlocfilehash: d02c1f7425372d60c10b40527dc5f0d65f923b45
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755784"
---
# <a name="dailyrecurrence"></a>DailyRecurrence

L’élément **DailyRecurrence** décrit la fréquence, en jours, dans laquelle un élément de calendrier ou d’une tâche est périodique. 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

**DailyRecurrencePatternType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Intervalle](interval.md) <br/> |Définit l’intervalle, en jours, entre deux éléments périodiques consécutives. La valeur doit être compris entre 1 et 999.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Périodicité (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de périodicité pour les tâches répétitives.  <br/> |
|[Périodicité (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité pour les éléments de calendrier et les demandes de réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

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

