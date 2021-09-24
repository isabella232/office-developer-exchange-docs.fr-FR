---
title: Mois
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: L’élément Month représente le mois de transition de l’année vers et depuis l’heure standard et l’heure d’été.
ms.openlocfilehash: aca81faf2767e17dab956db9a208245fbd0b7d83
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520429"
---
# <a name="month"></a>Mois

**L’élément Month** représente le mois de transition de l’année vers et depuis l’heure standard et l’heure d’été. 
  
```xml
<Month>...</Month>
```

 **Short**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [Bias (UTC).](bias-utc.md) Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée. <br/> <br/>  Les expressions XPath de l’élément StandardTime sont [les suivantes](standardtime.md) : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée. Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>  Les expressions XPath de [l’élément DaylightTime](daylighttime.md) sont les suivantes :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur représente le rang ordinal du mois par occurrence et doit être un nombre entre 1 et 12. Il s’agit d’un type de données d’un petit ensemble.
  
## <a name="remarks"></a>Remarques

Un [élément StandardTime](standardtime.md) qui contient un élément [DayOrder](dayorder.md) dont la valeur est 5, un élément **Month** avec une valeur de 10 et un élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) dont la valeur est Sunday signifie que la transition de l’heure standard à l’heure d’été a lieu le cinquième dimanche du dixième mois. 
  
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

