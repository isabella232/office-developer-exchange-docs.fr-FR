---
title: Mois
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
description: L’élément Month représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828476"
---
# <a name="month"></a>Mois

L’élément **Month** représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été. 
  
```xml
<Month>...</Month>
```

 **Court**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) . Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée. <br/> <br/>  Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>  Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur représente le rang ordinal du mois par occurrence et doit être un nombre compris entre 1 et 12. Il s’agit d’un type de données entier court.
  
## <a name="remarks"></a>Remarques

Un élément [StandardTime](standardtime.md) qui contient un élément [DayOrder](dayorder.md) qui a une valeur de 5, un élément **mois** qui a une valeur de 10 et un élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui a une valeur de dimanche signifie que la transition à partir de l’heure l’heure d’été se produit le dimanche cinquième du dixième mois. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

