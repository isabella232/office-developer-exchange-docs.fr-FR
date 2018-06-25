---
title: AdjacentMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetingCount
api_type:
- schema
ms.assetid: 35045024-f6e1-47d1-89be-f100b7b4f3c7
description: L’élément AdjacentMeetingCount représente le nombre total d’éléments de calendrier sont adjacents à une heure de réunion.
ms.openlocfilehash: a00468bec392498745fe778b627259a79d6027bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755184"
---
# <a name="adjacentmeetingcount"></a>AdjacentMeetingCount

L’élément **AdjacentMeetingCount** représente le nombre total d’éléments de calendrier sont adjacents à une heure de réunion. 
  
```xml
<AdjacentMeetingCount/>
```

 **Int**
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
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente un entier est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

