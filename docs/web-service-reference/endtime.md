---
title: EndTime
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
description: L’élément EndTime représente la fin d’une plage de temps.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462991"
---
# <a name="endtime"></a>EndTime

L’élément **EndTime** représente la fin d’une plage de temps. 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |Identifie la période interrogée pour les informations de disponibilité de l’utilisateur.<br/><br/> Voici l’expression XPath de cet élément :<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.<br/><br/> Voici l’expression XPath de cet élément :<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> | Spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**.  <br/><br/>  Voici les expressions XPath possibles pour cet élément :<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[Réunions](occurrence.md) <br/> |Représente une occurrence modifiée unique d’un élément de calendrier périodique.  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique. Cette information est utilisée pour les demandes de disponibilité. L’élément **EndTime** est requis dans l’élément **CalendarEvent** . L’élément **EndTime** de l’élément **CalendarEvent** est propre au type **CalendarEvent** .<br/><br/> Voici l’expression XPath de cet élément :<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise.
  
## <a name="remarks"></a>Remarques

L’élément [StartTime](starttime.md) représente le début d’une période. 
  
L’heure de fin représente l’heure du client.
  
Le schéma comprend de nombreux éléments [EndTime](endtime.md) . 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
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

