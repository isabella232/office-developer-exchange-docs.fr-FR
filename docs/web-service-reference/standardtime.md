---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: L’élément StandardTime représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément Bias (UTC). Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.
ms.openlocfilehash: ceddc511bf1883078c88dee240fc308d02024220
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544660"
---
# <a name="standardtime"></a>StandardTime

**L’élément StandardTime** représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [Bias (UTC).](bias-utc.md) Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée. 
  
- [TimeZone (Availability)](timezone-availability.md)
- [StandardTime](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 **SerializableTimeZoneTime**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Représente le décalage par rapport au décalage UTC identifié par l’élément [Bias (UTC)](bias-utc.md) pour l’heure standard et l’heure d’été. Cette valeur est exprimée en minutes.  <br/> |
|[Time](time.md) <br/> |Représente l’heure de transition de la journée vers et depuis l’heure standard et l’heure d’été.  <br/> |
|[DayOrder](dayorder.md) <br/> |Représente l’occurrence _n_th jour spécifiée dans l’élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) qui représente la date de transition entre l’heure standard et l’heure d’été.  <br/> |
|[Month](month.md) <br/> |Représente le mois de transition de l’année vers et depuis l’heure standard et l’heure d’été.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Représente le jour de la semaine au cours de la transition entre l’heure standard et l’heure d’été.  <br/> |
|[Année](year.md) <br/> |Définit un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TimeZone (Availability)](timezone-availability.md) <br/> | Contient des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été. <br/><br/>Les expressions XPath de cet élément sont les suivantes : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément StandardTime** représente un temps de décalage représenté par l’élément [Bias (UTC).](bias-utc.md) Lorsque [l’élément Bias](bias.md) enfant est égal à 0, l’heure standard est égale au décalage de décalage par rapport à l’UTC représenté par l’élément [Bias (UTC).](bias-utc.md) 
  
## <a name="example"></a>Exemple

L’exemple suivant illustre une région où l’heure d’été est observée. La transition entre l’heure d’été et l’heure standard est observée à 2 heures du matin. le cinquième dimanche du dixième mois.
  
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

