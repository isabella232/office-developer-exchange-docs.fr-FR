---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: L’élément MeetingWorkspaceUrl contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier. Un espace de travail de réunion est un site Web partagé pour la planification de la réunion et le suivi des résultats.
ms.openlocfilehash: c3d051d3529e9de9288c5ecaec2d601b317e2b0b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540796"
---
# <a name="meetingworkspaceurl"></a>MeetingWorkspaceUrl

**L’élément MeetingWorkspaceUrl** contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier. Un espace de travail de réunion est un site Web partagé pour la planification de la réunion et le suivi des résultats. 
  
```xml
<MeetingWorkspaceUrl/>
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
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une URL est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

La propriété MeetingWorkspaceUrl est accessible en lecture et en lecture pour l’élément de calendrier de l’organisateur. Il est en lecture seule pour les demandes de réunion et les éléments de calendrier des participants.
  
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

