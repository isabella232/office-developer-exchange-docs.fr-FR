---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: L’élément CalendarEventDetails fournit des informations supplémentaires sur un événement de calendrier.
ms.openlocfilehash: c332d17b1bb630b9635e64c484b4c5fd989f9845
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516089"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

**L’élément CalendarEventDetails fournit** des informations supplémentaires sur un événement de calendrier. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID](id.md) <br/> |Représente l’ID d’entrée de l’élément de calendrier.  <br/> |
|[Subject (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Représente l’objet de l’élément de calendrier.  <br/> |
|[Location (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Représente le champ d’emplacement de l’élément de calendrier.  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Indique si l’événement de calendrier est une réunion ou un rendez-vous.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Indique si l’événement de calendrier est une instance d’un élément de calendrier périodique ou d’un élément de calendrier unique.  <br/> |
|[IsException](isexception.md) <br/> |Indique si une instance d’un élément de calendrier périodique est modifiée à partir du maître.  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |Indique si un rappel a été définie pour l’événement de calendrier.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Indique si l’élément de calendrier est privé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Représente une occurrence d’élément de calendrier unique.  <br/> Voici l’expression XPath 2.0 à cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent. 
  
Si [l’élément IsPrivate](isprivate.md) est **vrai,** tous les autres éléments de l’élément [CalendarEventDetails](calendareventdetails.md) ne sont pas renvoyés dans la réponse. 
  
L’opération GetUserAvailability ne retourne pas d’informations détaillées sur l’appelant, sauf si l’appelant dispose d’un accès en lecture sur le calendrier de l’utilisateur cible. Vous pouvez définir des autorisations d’accès à l’aide Exchange Management Shell.
  
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

