---
title: EventTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: L’élément EventTypes contient une collection de types de notification d’événement qui sont utilisés pour créer un abonnement.
ms.openlocfilehash: 7ea783dc0bf73abf992616b1f86c7621c5b36fc8
ms.sourcegitcommit: 25cbbc6707e4ec0621c5c46baf7fe49be42d3297
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/07/2018
ms.locfileid: "25440836"
---
# <a name="eventtypes"></a><span data-ttu-id="35ac2-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="35ac2-103">EventTypes</span></span>

<span data-ttu-id="35ac2-104">L’élément **EventTypes** contient une collection de types de notification d’événement qui sont utilisés pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="35ac2-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="35ac2-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="35ac2-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35ac2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="35ac2-106">Attributes and elements</span></span>

<span data-ttu-id="35ac2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="35ac2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35ac2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="35ac2-108">Attributes</span></span>

<span data-ttu-id="35ac2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="35ac2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35ac2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="35ac2-110">Child elements</span></span>

|<span data-ttu-id="35ac2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="35ac2-111">**Element**</span></span>|<span data-ttu-id="35ac2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="35ac2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ac2-113">EventType</span><span class="sxs-lookup"><span data-stu-id="35ac2-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="35ac2-114">Représente un type de notification d’événement demandé est utilisé pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="35ac2-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35ac2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="35ac2-115">Parent elements</span></span>

|<span data-ttu-id="35ac2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="35ac2-116">**Element**</span></span>|<span data-ttu-id="35ac2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="35ac2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ac2-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="35ac2-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="35ac2-119">Représente un abonnement à un abonnement de notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="35ac2-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="35ac2-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="35ac2-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="35ac2-121">Représente un abonnement à un abonnement de notification push d’événements.</span><span class="sxs-lookup"><span data-stu-id="35ac2-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="35ac2-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="35ac2-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="35ac2-123">Représente un abonnement à un abonnement de notification d’événement diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="35ac2-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="35ac2-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="35ac2-124">Text value</span></span>

<span data-ttu-id="35ac2-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="35ac2-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="35ac2-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="35ac2-126">Remarks</span></span>

<span data-ttu-id="35ac2-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac2-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35ac2-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="35ac2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35ac2-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="35ac2-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35ac2-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="35ac2-130">Schema Name</span></span>  <br/> |<span data-ttu-id="35ac2-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="35ac2-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="35ac2-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="35ac2-132">Validation File</span></span>  <br/> |<span data-ttu-id="35ac2-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="35ac2-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35ac2-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="35ac2-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="35ac2-135">False</span><span class="sxs-lookup"><span data-stu-id="35ac2-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35ac2-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="35ac2-136">See also</span></span>



[<span data-ttu-id="35ac2-137">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="35ac2-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="35ac2-138">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="35ac2-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="35ac2-139">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="35ac2-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="35ac2-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="35ac2-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

