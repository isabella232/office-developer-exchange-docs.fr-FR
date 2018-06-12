---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: L’élément IsMeeting indique si l’élément de calendrier est une réunion ou un rendez-vous.
ms.openlocfilehash: bb1349a8690450882e6beac0ccd84a8d03272a7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828051"
---
# <a name="ismeeting"></a>IsMeeting

L’élément **IsMeeting** indique si l’élément de calendrier est une réunion ou un rendez-vous. 
  
```xml
<IsMeeting/>
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
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus. La valeur **true** indique que l’élément de calendrier est une réunion. La valeur **false** indique que l’élément de calendrier est un rendez-vous. 
  
## <a name="remarks"></a>Note

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

