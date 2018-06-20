---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: L’élément StatusEvent représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829592"
---
# <a name="statusevent"></a><span data-ttu-id="d3e63-103">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="d3e63-103">StatusEvent</span></span>

<span data-ttu-id="d3e63-104">L’élément **StatusEvent** représente une notification qu’aucune nouvelle activité se n’est produite dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d3e63-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="d3e63-105">**BaseNotificationEventType**</span><span class="sxs-lookup"><span data-stu-id="d3e63-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3e63-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3e63-106">Attributes and elements</span></span>

<span data-ttu-id="d3e63-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3e63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3e63-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3e63-108">Attributes</span></span>

<span data-ttu-id="d3e63-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3e63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3e63-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3e63-110">Child elements</span></span>

|<span data-ttu-id="d3e63-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3e63-111">**Element**</span></span>|<span data-ttu-id="d3e63-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3e63-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3e63-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="d3e63-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d3e63-114">Représente le dernier filigrane valid pour un abonnement.</span><span class="sxs-lookup"><span data-stu-id="d3e63-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3e63-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3e63-115">Parent elements</span></span>

|<span data-ttu-id="d3e63-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3e63-116">**Element**</span></span>|<span data-ttu-id="d3e63-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3e63-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3e63-118">Notification</span><span class="sxs-lookup"><span data-stu-id="d3e63-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d3e63-119">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="d3e63-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3e63-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3e63-120">Remarks</span></span>

<span data-ttu-id="d3e63-121">L’élément **StatusEvent** est retournée dans une notification pour les raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="d3e63-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="d3e63-122">Un client de type pull émet une demande de GetEvents sur un abonnement ayant aucune activité.</span><span class="sxs-lookup"><span data-stu-id="d3e63-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="d3e63-123">Un client push a pas d’événements dans la file d’attente lors de la [StatusFrequency](statusfrequency.md) a été atteinte.</span><span class="sxs-lookup"><span data-stu-id="d3e63-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="d3e63-124">**StatusEvent**[filigrane](watermark.md) est utilisé par une application cliente dans la même manière que les autres filigranes de type événement.</span><span class="sxs-lookup"><span data-stu-id="d3e63-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="d3e63-125">Toutefois, la limite pour le **StatusEvent** n’est pas le même que les filigranes utilisés pour d’autres événements.</span><span class="sxs-lookup"><span data-stu-id="d3e63-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="d3e63-126">Par exemple, un abonnement a des événements avec filigranes 1, 2 et 3 et les événements ont été communiquées correctement dans une notification.</span><span class="sxs-lookup"><span data-stu-id="d3e63-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="d3e63-127">Cet événement se produit une période d’inactivité et une demande **GetEvents** est envoyée.</span><span class="sxs-lookup"><span data-stu-id="d3e63-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="d3e63-128">Le serveur d’accès au Client (CAS) retourne un événement d’état et inclut le dernier filigrane, 3, comme le [PreviousWatermark](previouswatermark.md) et le cours [filigrane](watermark.md).</span><span class="sxs-lookup"><span data-stu-id="d3e63-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="d3e63-129">La limite pas restent les mêmes dans tous les cas.</span><span class="sxs-lookup"><span data-stu-id="d3e63-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="d3e63-130">Entrées d’événements sont conservées pendant 30 jours.</span><span class="sxs-lookup"><span data-stu-id="d3e63-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="d3e63-131">Pour maintenir un abonnement actif, les autorités de certification met régulièrement à jour les filigranes des files d’attente de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="d3e63-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="d3e63-132">Les filigranes mis à jour sont envoyées aux clients pour mettre à jour d’un abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="d3e63-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="d3e63-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d3e63-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3e63-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3e63-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3e63-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3e63-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3e63-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3e63-136">Schema name</span></span>  <br/> |<span data-ttu-id="d3e63-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d3e63-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3e63-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3e63-138">Validation file</span></span>  <br/> |<span data-ttu-id="d3e63-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3e63-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3e63-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3e63-140">Can be empty</span></span>  <br/> |<span data-ttu-id="d3e63-141">False</span><span class="sxs-lookup"><span data-stu-id="d3e63-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3e63-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3e63-142">See also</span></span>



[<span data-ttu-id="d3e63-143">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d3e63-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d3e63-144">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="d3e63-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d3e63-145">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d3e63-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)

