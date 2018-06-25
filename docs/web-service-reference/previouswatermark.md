---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: L’élément PreviousWatermark représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement.
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828886"
---
# <a name="previouswatermark"></a><span data-ttu-id="43baa-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="43baa-103">PreviousWatermark</span></span>

<span data-ttu-id="43baa-104">L’élément **PreviousWatermark** représente la limite du dernier événement qui a été correctement transmis au client pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="43baa-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="43baa-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="43baa-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43baa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="43baa-106">Attributes and elements</span></span>

<span data-ttu-id="43baa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="43baa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43baa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="43baa-108">Attributes</span></span>

<span data-ttu-id="43baa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43baa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43baa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="43baa-110">Child elements</span></span>

<span data-ttu-id="43baa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43baa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43baa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="43baa-112">Parent elements</span></span>

|<span data-ttu-id="43baa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43baa-113">**Element**</span></span>|<span data-ttu-id="43baa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="43baa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43baa-115">Notification</span><span class="sxs-lookup"><span data-stu-id="43baa-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="43baa-116">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="43baa-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43baa-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="43baa-117">Text value</span></span>

<span data-ttu-id="43baa-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="43baa-118">A text value is required.</span></span> <span data-ttu-id="43baa-119">La valeur de texte représente la limite le plus récent.</span><span class="sxs-lookup"><span data-stu-id="43baa-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="43baa-120">La valeur de texte ne peut pas être une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="43baa-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="43baa-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="43baa-121">Remarks</span></span>

<span data-ttu-id="43baa-122">La propriété **PreviousWatermark** est utile pour le client lors de la détermination de la dernière notification réussie.</span><span class="sxs-lookup"><span data-stu-id="43baa-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="43baa-123">Par exemple, si un abonnement a trois événements avec des filigranes 1, 2 et 3, et la prochaine notification est envoyée avec la valeur **PreviousWatermark** 3, le client peut comparer cette valeur à la limite supérieure de la dernière notification reçue.</span><span class="sxs-lookup"><span data-stu-id="43baa-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="43baa-124">Ainsi, le client à assurer la continuité des événements.</span><span class="sxs-lookup"><span data-stu-id="43baa-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="43baa-125">Pour les clients push, le **PreviousWatermark** est comparé à la limite connue dernière locale, côté client.</span><span class="sxs-lookup"><span data-stu-id="43baa-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="43baa-126">Si les valeurs sont différentes, le client a manqué une notification d’événement et doit rétablir un abonnement à l’aide de la dernière filigrane local.</span><span class="sxs-lookup"><span data-stu-id="43baa-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="43baa-127">Par exemple, si un client push reçoit trois événements pour un abonnement avec filigranes 1, 2 et 3, et la notification suivante est fourni avec une valeur **PreviousWatermark** 5, le client a manqué au moins une notification et doit créer un nouvel abonnement en passant un 3 en tant que filigrane.</span><span class="sxs-lookup"><span data-stu-id="43baa-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="43baa-128">Dans le cas d’un client extrait, la valeur de **PreviousWatermark** sera la même que le [filigrane](watermark.md) inclus par le client lors de l’appel GetEvents.</span><span class="sxs-lookup"><span data-stu-id="43baa-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="43baa-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="43baa-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43baa-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="43baa-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43baa-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="43baa-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43baa-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="43baa-132">Schema Name</span></span>  <br/> |<span data-ttu-id="43baa-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="43baa-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="43baa-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="43baa-134">Validation File</span></span>  <br/> |<span data-ttu-id="43baa-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43baa-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43baa-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="43baa-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="43baa-137">False</span><span class="sxs-lookup"><span data-stu-id="43baa-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43baa-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="43baa-138">See also</span></span>



[<span data-ttu-id="43baa-139">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="43baa-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="43baa-140">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="43baa-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="43baa-141">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="43baa-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

