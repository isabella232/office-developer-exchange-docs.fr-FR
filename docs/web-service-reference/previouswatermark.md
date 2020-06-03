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
description: L’élément PreviousWatermark représente le filigrane du dernier événement qui a été correctement communiqué au client pour l’abonnement.
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461652"
---
# <a name="previouswatermark"></a><span data-ttu-id="5a82c-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="5a82c-103">PreviousWatermark</span></span>

<span data-ttu-id="5a82c-104">L’élément **PreviousWatermark** représente le filigrane du dernier événement qui a été correctement communiqué au client pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="5a82c-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="5a82c-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="5a82c-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a82c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5a82c-106">Attributes and elements</span></span>

<span data-ttu-id="5a82c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5a82c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a82c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5a82c-108">Attributes</span></span>

<span data-ttu-id="5a82c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5a82c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a82c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5a82c-110">Child elements</span></span>

<span data-ttu-id="5a82c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5a82c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a82c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5a82c-112">Parent elements</span></span>

|<span data-ttu-id="5a82c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5a82c-113">**Element**</span></span>|<span data-ttu-id="5a82c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5a82c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a82c-115">Notification</span><span class="sxs-lookup"><span data-stu-id="5a82c-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5a82c-116">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="5a82c-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a82c-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5a82c-117">Text value</span></span>

<span data-ttu-id="5a82c-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="5a82c-118">A text value is required.</span></span> <span data-ttu-id="5a82c-119">La valeur texte représente le dernier filigrane.</span><span class="sxs-lookup"><span data-stu-id="5a82c-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="5a82c-120">La valeur de texte ne peut pas être une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="5a82c-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a82c-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="5a82c-121">Remarks</span></span>

<span data-ttu-id="5a82c-122">La propriété **PreviousWatermark** est utile au client pour déterminer la dernière notification réussie.</span><span class="sxs-lookup"><span data-stu-id="5a82c-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="5a82c-123">Par exemple, si un abonnement comporte trois événements avec les filigranes 1, 2 et 3, et que la notification suivante est envoyée avec une valeur **PreviousWatermark** de 3, le client peut comparer cette valeur à la valeur de filigrane de la dernière notification reçue.</span><span class="sxs-lookup"><span data-stu-id="5a82c-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="5a82c-124">Cela permet au client de s’assurer de la continuité des événements.</span><span class="sxs-lookup"><span data-stu-id="5a82c-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="5a82c-125">Pour les clients de type « poussé », le **PreviousWatermark** est comparé au dernier filigrane connu côté client et local.</span><span class="sxs-lookup"><span data-stu-id="5a82c-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="5a82c-126">Si les valeurs sont différentes, le client a manqué une notification d’événement et doit rétablir un abonnement à l’aide de la dernière limite locale.</span><span class="sxs-lookup"><span data-stu-id="5a82c-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="5a82c-127">Par exemple, si un client poussé reçoit trois événements pour un abonnement avec les filigranes 1, 2 et 3, et que la notification suivante est dotée d’une valeur **PreviousWatermark** de 5, le client a manqué au moins une notification et doit créer un nouvel abonnement, en passant un 3 comme filigrane.</span><span class="sxs-lookup"><span data-stu-id="5a82c-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="5a82c-128">Dans le cas d’un client de type pull, la valeur de **PreviousWatermark** sera identique à celle du [filigrane](watermark.md) fourni par le client dans l’appel GetEvents.</span><span class="sxs-lookup"><span data-stu-id="5a82c-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="5a82c-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5a82c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a82c-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5a82c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a82c-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5a82c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a82c-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5a82c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5a82c-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5a82c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a82c-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5a82c-134">Validation File</span></span>  <br/> |<span data-ttu-id="5a82c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a82c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a82c-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5a82c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a82c-137">False</span><span class="sxs-lookup"><span data-stu-id="5a82c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a82c-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5a82c-138">See also</span></span>



[<span data-ttu-id="5a82c-139">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5a82c-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5a82c-140">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="5a82c-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5a82c-141">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5a82c-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

