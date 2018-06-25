---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: L’élément DaysOfWeek indique les jours de la semaine qui sont utilisés dans l’élément périodicités.
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755829"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

L’élément **DaysOfWeek** indique les jours de la semaine qui sont utilisés dans l’élément périodicités. 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit une périodicité hebdomadaire.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs possibles sont les suivantes :
  
- Dimanche    
- Lundi    
- Mardi    
- Mercredi    
- Jeudi    
- Vendredi    
- Samedi    
- Day (cette valeur n’est pas valide pour une périodicité hebdomadaire)    
- WeekDay (cette valeur n’est pas valide pour une périodicité hebdomadaire)    
- WeekendDay (cette valeur n’est pas valide pour une périodicité hebdomadaire)
    
Une périodicité hebdomadaire peut contenir plusieurs valeurs. Les valeurs sont séparées par un espace. Par exemple, pour une périodicité hebdomadaire mardi et le jeudi, la valeur de texte sera « Mardi jeudi ».
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

