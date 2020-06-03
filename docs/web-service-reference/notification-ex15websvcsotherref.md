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
description: L’élément notification contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.
ms.openlocfilehash: c4a5206c14985ec46cf40162a9ce4eaec68242ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530386"
---
# <a name="notification"></a><span data-ttu-id="c10f7-103">Notification</span><span class="sxs-lookup"><span data-stu-id="c10f7-103">Notification</span></span>

<span data-ttu-id="c10f7-104">L’élément **notification** contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="c10f7-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
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

<span data-ttu-id="c10f7-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="c10f7-105">**NotificationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c10f7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c10f7-106">Attributes and elements</span></span>

<span data-ttu-id="c10f7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c10f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c10f7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c10f7-108">Attributes</span></span>

<span data-ttu-id="c10f7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c10f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c10f7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c10f7-110">Child elements</span></span>

|<span data-ttu-id="c10f7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c10f7-111">**Element**</span></span>|<span data-ttu-id="c10f7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c10f7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c10f7-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c10f7-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="c10f7-114">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="c10f7-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="c10f7-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="c10f7-116">Représente le filigrane du dernier événement qui a été correctement communiqué au client pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c10f7-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-117">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="c10f7-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="c10f7-118">Indique s’il existe d’autres événements dans la file d’attente à remettre au client.</span><span class="sxs-lookup"><span data-stu-id="c10f7-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="c10f7-120">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="c10f7-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="c10f7-122">Représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="c10f7-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="c10f7-124">Représente un événement dans lequel un élément ou un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="c10f7-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-125">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="c10f7-126">Représente un événement dans lequel un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="c10f7-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="c10f7-128">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="c10f7-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="c10f7-130">Représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c10f7-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="c10f7-132">Représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c10f7-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="c10f7-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="c10f7-134">Représente un événement dans lequel le temps de disponibilité d’un élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="c10f7-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c10f7-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c10f7-135">Parent elements</span></span>

|<span data-ttu-id="c10f7-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c10f7-136">**Element**</span></span>|<span data-ttu-id="c10f7-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="c10f7-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c10f7-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c10f7-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="c10f7-139">Contient l’État et le résultat d’une demande GetEvents unique.</span><span class="sxs-lookup"><span data-stu-id="c10f7-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="c10f7-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c10f7-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="c10f7-141">Contient l’État et le résultat d’une seule demande SendNotification.</span><span class="sxs-lookup"><span data-stu-id="c10f7-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c10f7-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c10f7-142">Text value</span></span>

<span data-ttu-id="c10f7-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c10f7-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c10f7-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="c10f7-144">Remarks</span></span>

<span data-ttu-id="c10f7-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c10f7-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c10f7-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c10f7-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c10f7-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c10f7-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c10f7-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c10f7-148">Schema Name</span></span>  <br/> |<span data-ttu-id="c10f7-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c10f7-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="c10f7-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c10f7-150">Validation File</span></span>  <br/> |<span data-ttu-id="c10f7-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c10f7-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c10f7-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c10f7-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="c10f7-153">False</span><span class="sxs-lookup"><span data-stu-id="c10f7-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c10f7-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c10f7-154">See also</span></span>

- [<span data-ttu-id="c10f7-155">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="c10f7-155">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="c10f7-156">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="c10f7-156">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="c10f7-157">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="c10f7-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) 
- [<span data-ttu-id="c10f7-158">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="c10f7-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)

