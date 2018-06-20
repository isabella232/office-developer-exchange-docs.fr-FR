---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: L’élément DaylightTime représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément Bias (UTC) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755818"
---
# <a name="daylighttime"></a>DaylightTime

L’élément **DaylightTime** représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard. 
  
- [Fuseau horaire (disponibilité)](timezone-availability.md) 
- [DaylightTime](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

**SerializableTimeZoneTime**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Représente le décalage de l’offset UTC identifié par l’élément [Bias (UTC)](bias-utc.md) heure standard et l’heure d’été. Cette valeur est exprimée en minutes.  <br/> |
|[Heure](time.md) <br/> |Représente le temps de transition de la journée à et d’heure standard et l’heure d’été.  <br/> |
|[DayOrder](dayorder.md) <br/> |Représente l’occurrence _n_th de la journée qui est spécifiée dans l’élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui représente la date de transition d’et à l’heure standard et l’heure d’été.  <br/> |
|[Mois](month.md) <br/> |Représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.  <br/> |
|[DayOfWeek (fuseau horaire)](dayofweek-timezone.md) <br/> |Représente le jour de la semaine quand se produit la transition vers et depuis l’heure standard et l’heure d’été.  <br/> |
|[Année](year.md) <br/> |Utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Fuseau horaire (disponibilité)](timezone-availability.md) <br/> | Contient des éléments qui identifient les informations de fuseau horaire.<br/><br/>Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>Exemple

La demande GetUserAvailability partielle suivante représente une application cliente dans un emplacement qui reconnaît l’heure d’été.
  
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

