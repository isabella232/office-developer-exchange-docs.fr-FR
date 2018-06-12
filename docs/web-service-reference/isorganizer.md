---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: L’élément IsOrganizer spécifie une valeur de type Boolean qui indique si cette personne est l’organisateur de la réunion.
ms.openlocfilehash: 5fd775cfc0a296c08d19d0468d96aa36ba67ddd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828063"
---
# <a name="isorganizer"></a>IsOrganizer

L’élément **IsOrganizer** spécifie une valeur de type Boolean qui indique si cette personne est l’organisateur de la réunion. 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **IsOrganizer** indique que le message du calendrier élément ou la réunion a été créé par l’utilisateur. La valeur **false** indique que le message du calendrier élément ou la réunion a été créé pas VC l’utilisateur. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

