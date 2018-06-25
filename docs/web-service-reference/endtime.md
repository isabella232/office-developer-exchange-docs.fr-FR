---
title: Heure de fin
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: L’élément EndTime représente la fin d’un intervalle de temps.
ms.openlocfilehash: 7d3d186618a7bcc05ad82532e13e03d2e67a0e40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756196"
---
# <a name="endtime"></a>Heure de fin

L’élément **EndTime** représente la fin d’un intervalle de temps. 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Durée](timewindow.md) <br/> |Identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> | Spécifie la durée pour laquelle le statut d’absence du bureau (OOF) est activé si l’élément [OofState](oofstate.md) est défini sur **planifiée**.  <br/><br/>  Les expressions XPath possibles de cet élément sont les suivantes :<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une seule occurrence de modification d’un élément de calendrier périodique.  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique. Il est utilisé pour les recherches de disponibilité. L’élément **EndTime** est requis dans l’élément **CalendarEvent** . L’élément de **l’heure de fin** dans l’élément **CalendarEvent** est unique pour le type **CalendarEvent** .<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise.
  
## <a name="remarks"></a>Remarques

L’élément [StartTime](starttime.md) représente le début d’un intervalle de temps. 
  
L’heure de fin représente la durée du client.
  
Le schéma inclut de nombreux éléments de [l’heure de fin](endtime.md) . 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
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

