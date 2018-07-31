---
title: Notification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: L’élément de Notification contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.
ms.openlocfilehash: 942ec18521fc484a7a3aa1385fb54f480ce9d11f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354350"
---
# <a name="notification"></a>Notification

L’élément de **Notification** contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification. 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

**NotificationType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Représente l’identificateur d’un abonnement.  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |Représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement.  <br/> |
|[MoreEvents](moreevents.md) <br/> |Indique s’il existe plusieurs événements dans la file d’attente pour être remis au client.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est créé.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est supprimé.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement auquel un élément ou un dossier est modifiée.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent à un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement qui est déclenché par un nouvel élément de messagerie dans une boîte aux lettres.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |Représente un événement dans lequel les temps de disponibilité d’un élément a été modifié.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contient l’état et les résultats d’une requête SendNotification.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération d'abonnement](subscribe-operation.md) 
- [Opération de GetEvents](getevents-operation.md) 
- [Opération de GetStreamingEvents](getstreamingevents-operation.md) 
- [Opération de résiliation d'abonnement](unsubscribe-operation.md)

