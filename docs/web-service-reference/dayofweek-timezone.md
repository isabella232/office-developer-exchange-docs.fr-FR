---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: L’élément DayOfWeek représente le jour de la semaine où la transition de fuseau horaire a lieu.
ms.openlocfilehash: 7bc05f417268ccfb20adae12e2694d8360023ab2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457843"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (TimeZone)

L’élément **DayOfWeek** représente le jour de la semaine où la transition de fuseau horaire a lieu. 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime Element](standardtime.md) <br/> | Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .<br/><br/>Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.<br/><br/>Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit chaque année.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte est représentée par une énumération qui a les valeurs possibles suivantes :
  
- Warm    
- Lundi    
- Mardi    
- Mercredi    
- Jeudi    
- Vendredi    
- Samedi    
- Day    
- Jour de la semaine   
- WeekendDay
    
## <a name="remarks"></a>Remarques

Un élément [StandardTime Element](standardtime.md) qui contient un élément [DayOrder](dayorder.md) ayant une valeur de 5, un élément [Month](month.md) qui a la valeur 10 et un élément **DayOfWeek** dont la valeur est dimanche signifie que la transition entre l’heure standard et l’heure d’été se produit le cinquième dimanche du dixième mois. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

