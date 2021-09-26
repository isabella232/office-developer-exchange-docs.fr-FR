---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: L’élément AllowNewTimeProposal indique si une nouvelle heure de réunion peut être proposée pour une réunion par un participant.
ms.openlocfilehash: 1acb95189e1949204a25f97a82770b88590df776
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543729"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

**L’élément AllowNewTimeProposal** indique si une nouvelle heure de réunion peut être proposée pour une réunion par un participant. 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur Boolean est requise. La valeur **true indique** qu’une nouvelle proposition pour l’heure de réunion peut être créée . La valeur **false indique** que les nouvelles propositions d’heure ne sont pas autorisées. L’organisateur définit cette valeur dans la demande de réunion. 
  
## <a name="remarks"></a>Remarques

La propriété AllowNewTimeProposal est accessible en lecture et en lecture pour l’élément de calendrier de l’organisateur. Il est en lecture seule pour les demandes de réunion et les éléments de calendrier des participants.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
> [!NOTE]
> Exchange Les services web ne prend pas en charge les nouveaux messages de proposition d’heure. Pour obtenir les propriétés liées aux nouveaux messages de proposition d’heure, utilisez des propriétés étendues. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

