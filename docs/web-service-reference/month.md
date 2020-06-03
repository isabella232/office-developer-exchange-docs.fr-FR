---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: L’élément month représente le mois de transition de l’année, de l’heure standard et de l’heure d’été.
ms.openlocfilehash: f102dca4ed9e833b9742844cfd612c81dfd05e70
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468620"
---
# <a name="month"></a>Month

L’élément **Month** représente le mois de transition de l’année, de l’heure standard et de l’heure d’été. 
  
```xml
<Month>...</Month>
```

 **Inférieure**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime Element](standardtime.md) <br/> | Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) . Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée. <br/> <br/>  Voici les expressions XPath de l’élément [StandardTime Element](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée. Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>  Voici les expressions XPath de l’élément [DaylightTime](daylighttime.md) :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur représente le rang ordinal du mois par occurrence et doit être un nombre compris entre 1 et 12. Il s’agit d’un type de données entier court.
  
## <a name="remarks"></a>Remarques

Un élément [StandardTime Element](standardtime.md) qui contient un élément [DayOrder](dayorder.md) ayant la valeur 5, un élément **Month** qui a la valeur 10 et un élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) ayant la valeur dimanche signifie que la transition entre l’heure standard et l’heure d’été a lieu le cinquième dimanche du dixième mois. 
  
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

