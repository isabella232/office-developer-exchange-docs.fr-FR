---
title: Heure de début
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: L’élément StartTime représente le début d’un intervalle de temps.
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829560"
---
# <a name="starttime"></a>Heure de début

L’élément **StartTime** représente le début d’un intervalle de temps. 
  
```xml
<StartTime/
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
|[Durée](timewindow.md) <br/> |Identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.  <br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.  <br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément : <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> | Spécifie la durée pour laquelle le statut d’absence du bureau (OOF) est activé si l’élément [OofState](oofstate.md) est défini sur **planifiée**.  <br/><br/>  Les expressions XPath possibles de cet élément sont les suivantes : <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique. Il est utilisé pour les recherches de disponibilité. L’élément **StartTime** est requis dans l’élément **CalendarEvent** . L’élément **StartTime** dans l’élément **CalendarEvent** est unique pour le type **CalendarEvent** bien qu’il contient les mêmes valeurs de facettes qui contiennent les éléments de **l’heure de début** dans le type de **durée** .  <br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise.
  
## <a name="remarks"></a>Remarques

L’élément [EndTime](endtime.md) représente la fin de l’intervalle de temps. 
  
Le schéma inclut de nombreux éléments de [l’heure de début](starttime.md) . 
  
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

