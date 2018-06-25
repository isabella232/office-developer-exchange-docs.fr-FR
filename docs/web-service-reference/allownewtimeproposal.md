---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: L’élément AllowNewTimeProposal indique si une nouvelle heure de réunion peut être proposée pour une réunion à un participant.
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755195"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

L’élément **AllowNewTimeProposal** indique si une nouvelle heure de réunion peut être proposée pour une réunion à un participant. 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise. La valeur **true** indique qu’une nouvelle proposition de l’heure de la réunion peut être créée ; la valeur **false** indique que les nouvelles propositions d’horaires ne sont pas autorisées. L’organisateur définit cette valeur dans la demande de réunion. 
  
## <a name="remarks"></a>Remarques

La propriété AllowNewTimeProposal est en lecture-écriture pour l’élément de calendrier de l’organisateur de la. Il est en lecture seule pour les demandes de réunion et des éléments de calendrier des participants.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
> [!NOTE]
> Services Web Exchange ne gère pas les nouveaux messages de proposition de temps. Pour obtenir les propriétés liées aux nouveaux messages de proposition de temps, utilisez les propriétés étendues. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

