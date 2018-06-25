---
title: S’abonner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: L’élément Subscribe contient les propriétés utilisées pour créer des abonnements.
ms.openlocfilehash: 9f23f566f9105c655b289ed9b434c5e7b917207f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829618"
---
# <a name="subscribe"></a><span data-ttu-id="c7c61-103">S’abonner</span><span class="sxs-lookup"><span data-stu-id="c7c61-103">Subscribe</span></span>

<span data-ttu-id="c7c61-104">L’élément **Subscribe** contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="c7c61-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="c7c61-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="c7c61-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7c61-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c7c61-106">Attributes and elements</span></span>

<span data-ttu-id="c7c61-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c7c61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7c61-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c7c61-108">Attributes</span></span>

<span data-ttu-id="c7c61-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c7c61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7c61-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c7c61-110">Child elements</span></span>

|<span data-ttu-id="c7c61-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c7c61-111">**Element**</span></span>|<span data-ttu-id="c7c61-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c7c61-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c61-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c7c61-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="c7c61-114">Représente un abonnement à une notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="c7c61-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="c7c61-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c7c61-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="c7c61-116">Représente un abonnement à une notification d’événement de type push.</span><span class="sxs-lookup"><span data-stu-id="c7c61-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="c7c61-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c7c61-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="c7c61-118">Représente un abonnement à une notification d’événement diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="c7c61-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7c61-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c7c61-119">Parent elements</span></span>

<span data-ttu-id="c7c61-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c7c61-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7c61-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="c7c61-121">Remarks</span></span>

<span data-ttu-id="c7c61-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7c61-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7c61-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c7c61-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7c61-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c7c61-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7c61-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c7c61-125">Schema name</span></span>  <br/> |<span data-ttu-id="c7c61-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c7c61-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c7c61-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c7c61-127">Validation file</span></span>  <br/> |<span data-ttu-id="c7c61-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c7c61-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7c61-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c7c61-129">Can be empty</span></span>  <br/> |<span data-ttu-id="c7c61-130">False</span><span class="sxs-lookup"><span data-stu-id="c7c61-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7c61-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c7c61-131">See also</span></span>



[<span data-ttu-id="c7c61-132">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="c7c61-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c7c61-133">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="c7c61-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c7c61-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="c7c61-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="c7c61-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="c7c61-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

