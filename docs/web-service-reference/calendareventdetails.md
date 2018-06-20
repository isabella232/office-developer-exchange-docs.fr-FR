---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: L’élément CalendarEventDetails fournit des informations supplémentaires sur un événement de calendrier.
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755465"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

L’élément **CalendarEventDetails** fournit des informations supplémentaires sur un événement de calendrier. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 **CalendarEventDetails**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID](id.md) <br/> |Représente l’identificateur d’entrée de l’élément de calendrier.  <br/> |
|[Sujet (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Représente l’objet de l’élément de calendrier.  <br/> |
|[Emplacement (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Représente le champ emplacement de l’élément de calendrier.  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Indique si l’événement du calendrier est une réunion ou un rendez-vous.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Indique si l’événement du calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.  <br/> |
|[IsException](isexception.md) <br/> |Indique si une instance d’un élément de calendrier périodique est modifiée à partir de la forme de base.  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |Indique si un rappel a été défini pour l’événement de calendrier.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Indique si l’élément de calendrier est privé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique.  <br/> Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent. 
  
Si l’élément [IsPrivate](isprivate.md) a la **valeur true**, tous les autres éléments dans l’élément [CalendarEventDetails](calendareventdetails.md) ne sont pas renvoyés dans la réponse. 
  
L’opération GetUserAvailability ne renvoie pas d’informations détaillées sur l’appelant, sauf si l’appelant dispose d’un accès en lecture sur le calendrier de l’utilisateur cible. Vous pouvez définir des autorisations d’accès à l’aide de l’environnement Exchange Management Shell.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

