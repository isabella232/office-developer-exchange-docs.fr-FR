---
title: Periods
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: L’élément Periods représente un tableau de périodes qui définissent le décalage horaire à différentes étapes du fuseau horaire.
ms.openlocfilehash: e4a614c71e7194dd85db740da1796b69d9f25d69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515312"
---
# <a name="periods"></a>Periods

**L’élément Periods** représente un tableau de périodes qui définissent le décalage horaire à différentes étapes du fuseau horaire. 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 **NonEmptyArrayOfPeriodsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Period](period.md) <br/> |Définit le nom, le décalage horaire et l’identificateur unique d’une étape spécifique du fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Définit le fuseau horaire pour l’heure de début d’un [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Définit le fuseau horaire pour l’heure de fin d’un [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Définit un fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

