---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: L’élément CalendarEvent représente une occurrence d’élément de calendrier unique.
ms.openlocfilehash: fd57517595659f2081c82fe9f4665ce2c39059fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514822"
---
# <a name="calendarevent"></a>CalendarEvent

**L’élément CalendarEvent** représente une occurrence d’élément de calendrier unique. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 **CalendarEvent**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Représente le début d’un événement de calendrier. Il s’agit d’un élément enfant obligatoire.  <br/> |
|[EndTime](endtime.md) <br/> |Représente la fin d’un événement de calendrier. Il s’agit d’un élément enfant obligatoire.  <br/> |
|[BusyType](busytype.md) <br/> |Représente l’état de libre/occupé d’un événement de calendrier. Il s’agit d’un élément enfant obligatoire.  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |Fournit des informations supplémentaires pour un événement de calendrier. Il s’agit d’un élément enfant facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |Contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.  <br/> Voici l’expression XPath 2.0 à cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>Remarques

Les heures de rendez-vous et de réunion sont renvoyées dans le fuseau horaire du client. Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent. Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

