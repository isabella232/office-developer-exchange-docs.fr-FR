---
title: Fuseau horaire (disponibilité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: L’élément TimeZone contienne des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838741"
---
# <a name="timezone-availability"></a>Fuseau horaire (disponibilité)

L’élément **TimeZone** contienne des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |Représente le décalage général du temps universel coordonné (UTC). Cette valeur est exprimée en minutes.  <br/> |
|[StandardTime](standardtime.md) <br/> |Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) . Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur. Il s’agit d’un élément racine.  <br/> L’élément de **fuseau horaire** dans le message GetUserAvailabilityRequest représente le fuseau horaire dans lequel les valeurs DateTime dans la demande sont spécifiés. Les valeurs DateTime renvoyées par le service de disponibilité sont également dans ce fuseau horaire.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.  <br/> L’élément de **fuseau horaire** dans le message GetUserAvailabilityResponse représente les paramètres de fuseau horaire de l’utilisateur de boîte aux lettres demandée.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis dans l’élément [GetUserAvailabilityRequest](getuseravailabilityrequest.md) . Cet élément se produit une fois au maximum ou minimum fois lorsque l’élément parent est l’élément [WorkingHours](workinghours-ex15websvcsotherref.md) . 
  
## <a name="example"></a>Exemple

L’exemple suivant montre une partie d’une requête XML qui identifie un décalage de l’heure UTC de 8 heures dans l’application cliente.
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
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



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

