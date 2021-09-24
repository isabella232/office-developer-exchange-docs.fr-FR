---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: L’élément Bias représente le décalage par rapport au décalage UTC (Coordinated Universal Time) identifié par l’élément Bias (UTC) pour l’heure standard et l’heure d’été. Cette valeur est exprimée en minutes.
ms.openlocfilehash: 557605380dbda8c980272edcf445bb8099e14ada
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516096"
---
# <a name="bias"></a>Bias

**L’élément Bias** représente le décalage par rapport au décalage UTC (Coordinated Universal Time) identifié par l’élément [Bias (UTC)](bias-utc.md) pour l’heure standard et l’heure d’été. Cette valeur est exprimée en minutes. 
  
```xml
<Bias>...</Bias>
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
|[StandardTime](standardtime.md) <br/> | Représente un décalage par rapport à l’heure UTC représentée par l’élément [Bias (UTC).](bias-utc.md) Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.<br/><br/>Les expressions XPath de l’élément StandardTime sont [les suivantes](standardtime.md) :<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Représente un décalage par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée. Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.  <br/><br/>Les expressions XPath de [l’élément DaylightTime](daylighttime.md) sont les suivantes :<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte représente un integer.
  
## <a name="remarks"></a>Remarques

Le décalage utilisé pour déterminer l’heure locale ne peut être fourni que par l’un des **éléments Bias.** La somme des valeurs de l’élément Bias fournie par l’élément [DaylightTime](daylighttime.md) ou [l’élément StandardTime](standardtime.md) plus l’élément [Bias (UTC)](bias-utc.md) identifie l’heure locale. 
  
## <a name="example"></a>Exemple

L’exemple suivant montre une partie d’une demande XML qui identifie un utilisateur qui observe l’heure d’été en ajustant le décalage de -60 minutes par rapport à l’heure UTC. Cela rend effectivement le biais à 420 minutes de l’heure UTC.
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

