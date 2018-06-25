---
title: Heure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: L’élément heure représente le temps de transition de la journée à et d’heure standard et l’heure d’été.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838700"
---
# <a name="time"></a>Heure

L’élément **heure** représente le temps de transition de la journée à et d’heure standard et l’heure d’été. 
  
```xml
<Time>...</Time>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) . Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.  <br/><br/>  Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>  Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente les heures, minutes et secondes sous la forme suivante : hh : mm :.
  
## <a name="remarks"></a>Remarques

En cas de l’élément de **temps** dans l’élément [DaylightTime](daylighttime.md) , il représente l’heure du jour qui se produit la transition à partir de l’heure d’été à l’heure standard. En cas de l’élément de [temps](time.md) dans l’élément [StandardTime](standardtime.md) , il représente l’heure du jour qui se produit la transition à partir de l’heure standard à l’heure d’été. 
  
Cet élément a une occurrence minimale de zéro et une occurrence d’un maximum.
  
## <a name="example"></a>Exemple

La partie suivante d’une demande représente un temps de transition de 2 heures. à partir de l’heure standard à l’heure d’été.
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

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

