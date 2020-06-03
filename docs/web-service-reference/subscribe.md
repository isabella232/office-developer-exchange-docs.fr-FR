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
description: L’élément subscribe contient les propriétés utilisées pour créer des abonnements.
ms.openlocfilehash: f60e67654fb6af76e8081036a3463f5be401862d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530957"
---
# <a name="subscribe"></a><span data-ttu-id="5c23b-103">S’abonner</span><span class="sxs-lookup"><span data-stu-id="5c23b-103">Subscribe</span></span>

<span data-ttu-id="5c23b-104">L’élément **subscribe** contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="5c23b-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="5c23b-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="5c23b-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c23b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5c23b-106">Attributes and elements</span></span>

<span data-ttu-id="5c23b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5c23b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c23b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5c23b-108">Attributes</span></span>

<span data-ttu-id="5c23b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5c23b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c23b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5c23b-110">Child elements</span></span>

|<span data-ttu-id="5c23b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5c23b-111">**Element**</span></span>|<span data-ttu-id="5c23b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c23b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c23b-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="5c23b-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="5c23b-114">Représente un abonnement à une notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="5c23b-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="5c23b-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="5c23b-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="5c23b-116">Représente un abonnement à une notification d’événement par transmission.</span><span class="sxs-lookup"><span data-stu-id="5c23b-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="5c23b-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="5c23b-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="5c23b-118">Représente un abonnement à une notification d’événement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="5c23b-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c23b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5c23b-119">Parent elements</span></span>

<span data-ttu-id="5c23b-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c23b-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c23b-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="5c23b-121">Remarks</span></span>

<span data-ttu-id="5c23b-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c23b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c23b-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5c23b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c23b-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5c23b-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c23b-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5c23b-125">Schema name</span></span>  <br/> |<span data-ttu-id="5c23b-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5c23b-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c23b-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5c23b-127">Validation file</span></span>  <br/> |<span data-ttu-id="5c23b-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5c23b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c23b-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5c23b-129">Can be empty</span></span>  <br/> |<span data-ttu-id="5c23b-130">False</span><span class="sxs-lookup"><span data-stu-id="5c23b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c23b-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5c23b-131">See also</span></span>



[<span data-ttu-id="5c23b-132">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5c23b-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5c23b-133">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="5c23b-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5c23b-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="5c23b-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="5c23b-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5c23b-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

