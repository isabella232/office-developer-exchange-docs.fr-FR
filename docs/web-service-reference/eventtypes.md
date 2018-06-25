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
ms.openlocfilehash: f4c622376f6b607ed390511d7bb5f0f723889420
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756222"
---
# <a name="eventtypes"></a><span data-ttu-id="a9186-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="a9186-103">EventTypes</span></span>

<span data-ttu-id="a9186-104">L’élément **EventTypes** contient une collection de types de notification d’événement qui sont utilisés pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="a9186-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="a9186-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="a9186-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9186-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a9186-106">Attributes and elements</span></span>

<span data-ttu-id="a9186-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a9186-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9186-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a9186-108">Attributes</span></span>

<span data-ttu-id="a9186-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a9186-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9186-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a9186-110">Child elements</span></span>

|<span data-ttu-id="a9186-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a9186-111">**Element**</span></span>|<span data-ttu-id="a9186-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a9186-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9186-113">EventType</span><span class="sxs-lookup"><span data-stu-id="a9186-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="a9186-114">Représente un type de notification d’événement demandé est utilisé pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="a9186-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9186-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a9186-115">Parent elements</span></span>

|<span data-ttu-id="a9186-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a9186-116">**Element**</span></span>|<span data-ttu-id="a9186-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a9186-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9186-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a9186-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="a9186-119">Représente un abonnement à un abonnement de notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="a9186-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="a9186-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a9186-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="a9186-121">Représente un abonnement à un abonnement de notification push d’événements.</span><span class="sxs-lookup"><span data-stu-id="a9186-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="a9186-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a9186-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="a9186-123">Représente un abonnement à un abonnement de notification d’événement diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="a9186-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9186-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a9186-124">Text value</span></span>

<span data-ttu-id="a9186-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a9186-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a9186-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="a9186-126">Remarks</span></span>

<span data-ttu-id="a9186-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9186-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9186-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a9186-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9186-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a9186-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9186-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a9186-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a9186-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a9186-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9186-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a9186-132">Validation File</span></span>  <br/> |<span data-ttu-id="a9186-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a9186-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9186-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a9186-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9186-135">False</span><span class="sxs-lookup"><span data-stu-id="a9186-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9186-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a9186-136">See also</span></span>



[<span data-ttu-id="a9186-137">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a9186-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a9186-138">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="a9186-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="a9186-139">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a9186-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="a9186-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a9186-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

