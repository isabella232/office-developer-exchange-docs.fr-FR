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
description: L’élément Interval définit l’intervalle entre deux éléments périodiques consécutifs.
ms.openlocfilehash: 70a41cfc438f057cbe11d792f0004d46d0abcc85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526563"
---
# <a name="interval"></a>Intervalle

L’élément **Interval** définit l’intervalle entre deux éléments périodiques consécutifs. 
  
```xml
<Interval/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Représente une périodicité mensuelle.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Décrit la fréquence, en jours, de régénération d’une tâche.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Décrit la fréquence, en jours, de récurrence d’une tâche.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Décrit la fréquence, en mois, de régénération d’une tâche.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit un modèle mensuel relatif pour une tâche périodique.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit la fréquence, en semaines, et les jours de récurrence d’une tâche.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Décrit la fréquence, en semaines, de régénération d’une tâche.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Décrit la fréquence de régénération d’une tâche, exprimée en années.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un entier est requise.
  
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

