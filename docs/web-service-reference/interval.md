---
title: Intervalle
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: L’élément intervalle définit l’intervalle entre deux éléments périodiques consécutives.
ms.openlocfilehash: 55d26b5b1b51aca3effa93a2e6852c1ae57ef4b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827962"
---
# <a name="interval"></a>Intervalle

L’élément **intervalle** définit l’intervalle entre deux éléments périodiques consécutives. 
  
```xml
<Interval/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Représente une périodicité mensuelle.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Décrit la fréquence, en jours, dans laquelle une tâche est régénérée.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Décrit la fréquence, en jours, dans laquelle une tâche est périodique.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Décrit la fréquence, en mois, dans lequel une tâche est régénérée.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit un modèle mensuel relatif pour une tâche périodique.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit la fréquence, en semaines, et les jours où une tâche est périodique.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Décrit la fréquence, en semaines, dans lequel une tâche est régénérée.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Décrit la fréquence, en années, dans lequel une tâche est régénérée.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente un entier est requise.
  
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

