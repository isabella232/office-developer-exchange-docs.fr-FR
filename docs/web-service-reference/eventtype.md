---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: L’élément EventType est utilisé pour créer un abonnement et identifie un type d’événement à signalé dans une notification.
ms.openlocfilehash: 7378ba45b155281df9e00ad635b7c6970a270f2c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545215"
---
# <a name="eventtype"></a>EventType

**L’élément EventType** est utilisé pour créer un abonnement et identifie un type d’événement à signalé dans une notification. 
  
```xml
<EventType/>
```

 **NotificationEventTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[EventTypes](eventtypes.md) <br/> |Contient une collection de types d’événements de notification d’événement qui sont utilisés pour créer un abonnement.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- CopiedEvent
    
- CreatedEvent
    
- DeletedEvent
    
- ModifiedEvent
    
- MovedEvent
    
- NewMailEvent
    
- FreeBusyChangedEvent
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

