---
title: TimeZone (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: L’élément TimeZone contient des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.
ms.openlocfilehash: 7ca6f0f2d9950770055d19c04adab9b76b95c295
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538841"
---
# <a name="timezone-availability"></a>TimeZone (Availability)

**L’élément TimeZone** contient des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |Représente le décalage général par rapport au temps universel coordonné (UTC). Cette valeur est exprimée en minutes.  <br/> |
|[StandardTime](standardtime.md) <br/> |Représente un décalage par rapport à l’heure UTC représentée par l’élément [Bias (UTC).](bias-utc.md) Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Représente un décalage par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée. Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.  <br/> **L’élément TimeZone** dans le message GetUserAvailabilityRequest représente le fuseau horaire dans lequel les valeurs DateTime dans la demande sont spécifiées. Les valeurs DateTime renvoyées par le service de disponibilité sont également dans ce fuseau horaire.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.  <br/> **L’élément TimeZone** dans le message GetUserAvailabilityResponse représente les paramètres de fuseau horaire de l’utilisateur de boîte aux lettres demandé.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis dans [l’élément GetUserAvailabilityRequest.](getuseravailabilityrequest.md) Cet élément se produit au plus une fois ou au moins zéro fois lorsque l’élément parent est [l’élément WorkingHours.](workinghours-ex15websvcsotherref.md) 
  
## <a name="example"></a>Exemple

L’exemple suivant montre une partie d’une demande XML qui identifie un décalage par rapport à 8 heures UTC dans l’application cliente.
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

