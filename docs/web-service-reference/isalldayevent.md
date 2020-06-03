---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: L’élément IsAllDayEvent indique si un élément de calendrier ou une demande de réunion représente un événement d’une journée entière.
ms.openlocfilehash: f0c975deecf96e94599a47ef2c33e54a7d1a80b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526535"
---
# <a name="isalldayevent"></a>IsAllDayEvent

L’élément **IsAllDayEvent** indique si un élément de calendrier ou une demande de réunion représente un événement d’une journée entière. 
  
```xml
<IsAllDayEvent/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur booléenne est requise si cet élément est inclus. La valeur **true** indique que l’élément représente un événement d’une journée entière. La valeur **false** indique que l’élément s’étend sur une durée inférieure aux heures de travail d’un utilisateur. 
  
## <a name="remarks"></a>Remarques

Un événement d’une journée entière s’étend sur la durée des heures de travail définies pour une boîte aux lettres.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

