---
title: Emplacement (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: L’élément location représente le champ d’emplacement de l’élément de calendrier.
ms.openlocfilehash: 4a590c315d2211ce9128305a514e68f1c785596c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467997"
---
# <a name="location-calendareventdetails"></a>Emplacement (CalendarEventDetails)

L’élément **location** représente le champ d’emplacement de l’élément de calendrier. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
[Emplacement (CalendarEventDetails)](location-calendareventdetails.md)
  
```xml
<Location/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarEventDetails](calendareventdetails.md) <br/> |Fournit des informations supplémentaires pour un événement de calendrier.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est renvoyé dans la réponse. Cet élément peut contenir une chaîne vide. Cet élément est facultatif si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé. 
  
## <a name="remarks"></a>Remarques

Cet élément est mappé à une propriété nommée MAPI PR_Location.
  
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

