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
ms.openlocfilehash: a769d8988eb68d0fa0b02f3838cd891e714571b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828547"
---
# <a name="notification"></a><span data-ttu-id="ad279-103">Notification</span><span class="sxs-lookup"><span data-stu-id="ad279-103">Notification</span></span>

<span data-ttu-id="ad279-104">L’élément de **Notification** contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="ad279-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

 <span data-ttu-id="ad279-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="ad279-105">**NotificationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad279-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad279-106">Attributes and elements</span></span>

<span data-ttu-id="ad279-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad279-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad279-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad279-108">Attributes</span></span>

<span data-ttu-id="ad279-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad279-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad279-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad279-110">Child elements</span></span>

|<span data-ttu-id="ad279-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad279-111">**Element**</span></span>|<span data-ttu-id="ad279-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad279-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad279-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="ad279-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="ad279-114">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="ad279-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="ad279-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="ad279-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="ad279-116">Représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ad279-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="ad279-117">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="ad279-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="ad279-118">Indique s’il existe plusieurs événements dans la file d’attente pour être remis au client.</span><span class="sxs-lookup"><span data-stu-id="ad279-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="ad279-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="ad279-120">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="ad279-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="ad279-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="ad279-122">Représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="ad279-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="ad279-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="ad279-124">Représente un événement dans lequel un élément ou un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="ad279-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="ad279-125">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="ad279-126">Représente un événement auquel un élément ou un dossier est modifiée.</span><span class="sxs-lookup"><span data-stu-id="ad279-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="ad279-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="ad279-128">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent à un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="ad279-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="ad279-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="ad279-130">Représente un événement qui est déclenché par un nouvel élément de messagerie dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad279-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad279-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="ad279-132">Représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad279-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad279-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="ad279-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="ad279-134">Représente un événement dans lequel les temps de disponibilité d’un élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="ad279-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad279-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad279-135">Parent elements</span></span>

|<span data-ttu-id="ad279-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad279-136">**Element**</span></span>|<span data-ttu-id="ad279-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad279-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad279-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad279-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="ad279-139">Contient l’état et les résultats d’une seule demande GetEvents.</span><span class="sxs-lookup"><span data-stu-id="ad279-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="ad279-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad279-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="ad279-141">Contient l’état et les résultats d’une requête SendNotification.</span><span class="sxs-lookup"><span data-stu-id="ad279-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad279-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad279-142">Text value</span></span>

<span data-ttu-id="ad279-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad279-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad279-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad279-144">Remarks</span></span>

<span data-ttu-id="ad279-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad279-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad279-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad279-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad279-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad279-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad279-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad279-148">Schema Name</span></span>  <br/> |<span data-ttu-id="ad279-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ad279-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad279-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad279-150">Validation File</span></span>  <br/> |<span data-ttu-id="ad279-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad279-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad279-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad279-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad279-153">False</span><span class="sxs-lookup"><span data-stu-id="ad279-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad279-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad279-154">See also</span></span>



[<span data-ttu-id="ad279-155">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ad279-155">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ad279-156">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="ad279-156">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="ad279-157">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="ad279-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="ad279-158">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ad279-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)

