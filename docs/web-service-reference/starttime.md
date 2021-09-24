---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: L’élément StartTime représente le début d’une période.
ms.openlocfilehash: e6d9034fa1b01f0f0969837761f4da7c36cea752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531652"
---
# <a name="starttime"></a>StartTime

**L’élément StartTime** représente le début d’une période. 
  
```xml
<StartTime/
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
|[TimeWindow](timewindow.md) <br/> |Identifie l’étendue de temps à interroger pour les informations de disponibilité de l’utilisateur.  <br/><br/> Voici l’expression XPath de cet élément :  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’étendue de temps à interroger pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/><br/> Voici l’expression XPath de cet élément : <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> | Spécifie la durée pendant laquelle l’état Hors Office (OOF) est activé si l’élément [OofState](oofstate.md) est définie sur **Scheduled**.  <br/><br/>  Voici les expressions XPath possibles pour cet élément : <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique. Il est utilisé pour les demandes de disponibilité. **L’élément StartTime** est requis dans **l’élément CalendarEvent.** **L’élément StartTime** dans l’élément **CalendarEvent** est unique au type **CalendarEvent,** bien qu’il contienne les mêmes valeurs de facette que les éléments **StartTime** dans le type **Duration.**  <br/><br/> Voici l’expression XPath de cet élément :  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise.
  
## <a name="remarks"></a>Remarques

[L’élément EndTime](endtime.md) représente la fin de l’intervalle de temps. 
  
Le schéma inclut de nombreux [éléments StartTime.](starttime.md) 
  
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

