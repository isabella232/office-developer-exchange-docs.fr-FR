---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: L’élément Bias représente le décalage de l’offset de temps universel coordonné (UTC) identifié par l’élément Bias (UTC) heure standard et l’heure d’été. Cette valeur est exprimée en minutes.
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755389"
---
# <a name="bias"></a>Bias

L’élément **Bias** représente le décalage de l’offset de temps universel coordonné (UTC) identifié par l’élément [Bias (UTC)](bias-utc.md) heure standard et l’heure d’été. Cette valeur est exprimée en minutes. 
  
```xml
<Bias>...</Bias>
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
|[StandardTime](standardtime.md) <br/> | Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) . Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.<br/><br/>Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes :<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte représente un entier.
  
## <a name="remarks"></a>Remarques

Le décalage permet de déterminer l’heure locale seulement peut être assurée par un des éléments de **l’écart** . La somme des valeurs de l’élément Bias fournies par l’élément [DaylightTime](daylighttime.md) ou l’élément [StandardTime](standardtime.md) ainsi que l’élément [Bias (UTC)](bias-utc.md) identifie l’heure locale. 
  
## <a name="example"></a>Exemple

L’exemple suivant montre une partie d’une requête XML qui identifie un utilisateur qui observe l’heure d’été en ajustant le décalage de l’heure UTC à 60 minutes. Cela rend l’écart 420 minutes à l’heure UTC.
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
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

