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
description: L’élément StatusEvent représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468256"
---
# <a name="statusevent"></a><span data-ttu-id="980fa-103">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="980fa-103">StatusEvent</span></span>

<span data-ttu-id="980fa-104">L’élément **StatusEvent** représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="980fa-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="980fa-105">**BaseNotificationEventType**</span><span class="sxs-lookup"><span data-stu-id="980fa-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="980fa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="980fa-106">Attributes and elements</span></span>

<span data-ttu-id="980fa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="980fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="980fa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="980fa-108">Attributes</span></span>

<span data-ttu-id="980fa-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="980fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="980fa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="980fa-110">Child elements</span></span>

|<span data-ttu-id="980fa-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="980fa-111">**Element**</span></span>|<span data-ttu-id="980fa-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="980fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="980fa-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="980fa-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="980fa-114">Représente le dernier filigrane valide d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="980fa-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="980fa-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="980fa-115">Parent elements</span></span>

|<span data-ttu-id="980fa-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="980fa-116">**Element**</span></span>|<span data-ttu-id="980fa-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="980fa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="980fa-118">Notification</span><span class="sxs-lookup"><span data-stu-id="980fa-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="980fa-119">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="980fa-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="980fa-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="980fa-120">Remarks</span></span>

<span data-ttu-id="980fa-121">L’élément **StatusEvent** est renvoyé dans une notification pour l’une des raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="980fa-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="980fa-122">Un client de réception émet une demande GetEvents sur un abonnement qui n’a aucune activité.</span><span class="sxs-lookup"><span data-stu-id="980fa-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="980fa-123">Un client poussé n’a pas d’événements dans la file d’attente lorsque le [StatusFrequency](statusfrequency.md) est atteint.</span><span class="sxs-lookup"><span data-stu-id="980fa-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="980fa-124">Le **StatusEvent**[filigrane](watermark.md) StatusEvent est utilisé par une application cliente de la même manière que les autres filigranes de type d’événement.</span><span class="sxs-lookup"><span data-stu-id="980fa-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="980fa-125">Toutefois, le filigrane de l' **StatusEvent** n’est pas le même que les filigranes utilisés pour d’autres événements.</span><span class="sxs-lookup"><span data-stu-id="980fa-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="980fa-126">Par exemple, un abonnement comporte des événements avec les filigranes 1, 2 et 3 et ces événements ont été correctement communiqués dans une notification.</span><span class="sxs-lookup"><span data-stu-id="980fa-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="980fa-127">Une période d’inactivité se produit et une demande **GetEvents** est envoyée.</span><span class="sxs-lookup"><span data-stu-id="980fa-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="980fa-128">Le serveur d’accès au client (CAS) renvoie un événement d’État et inclut le dernier filigrane, 3, à la fois [PreviousWatermark](previouswatermark.md) et le [filigrane](watermark.md)actuel.</span><span class="sxs-lookup"><span data-stu-id="980fa-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="980fa-129">Le filigrane ne reste pas le même dans tous les cas.</span><span class="sxs-lookup"><span data-stu-id="980fa-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="980fa-130">Les entrées d’événement sont conservées pendant 30 jours.</span><span class="sxs-lookup"><span data-stu-id="980fa-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="980fa-131">Pour maintenir un abonnement actif, le CAS met régulièrement à jour les filigranes pour les files d’attente des abonnements.</span><span class="sxs-lookup"><span data-stu-id="980fa-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="980fa-132">Les filigranes mis à jour sont envoyés aux clients pour maintenir un abonnement actif.</span><span class="sxs-lookup"><span data-stu-id="980fa-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="980fa-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="980fa-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="980fa-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="980fa-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="980fa-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="980fa-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="980fa-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="980fa-136">Schema name</span></span>  <br/> |<span data-ttu-id="980fa-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="980fa-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="980fa-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="980fa-138">Validation file</span></span>  <br/> |<span data-ttu-id="980fa-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="980fa-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="980fa-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="980fa-140">Can be empty</span></span>  <br/> |<span data-ttu-id="980fa-141">False</span><span class="sxs-lookup"><span data-stu-id="980fa-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="980fa-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="980fa-142">See also</span></span>



[<span data-ttu-id="980fa-143">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="980fa-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="980fa-144">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="980fa-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="980fa-145">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="980fa-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)

