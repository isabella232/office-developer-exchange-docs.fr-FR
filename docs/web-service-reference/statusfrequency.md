---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: L’élément StatusFrequency représente la valeur du délai d’attente maximale, en minutes, dans laquelle les nouvelles tentatives sont effectuées par le serveur.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829589"
---
# <a name="statusfrequency"></a><span data-ttu-id="9b1de-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="9b1de-103">StatusFrequency</span></span>

<span data-ttu-id="9b1de-104">L’élément **StatusFrequency** représente la valeur du délai d’attente maximale, en minutes, dans laquelle les nouvelles tentatives sont effectuées par le serveur.</span><span class="sxs-lookup"><span data-stu-id="9b1de-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="9b1de-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="9b1de-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="9b1de-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="9b1de-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="9b1de-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="9b1de-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="9b1de-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="9b1de-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b1de-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b1de-109">Attributes and elements</span></span>

<span data-ttu-id="9b1de-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b1de-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b1de-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b1de-111">Attributes</span></span>

<span data-ttu-id="9b1de-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b1de-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b1de-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b1de-113">Child elements</span></span>

<span data-ttu-id="9b1de-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b1de-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b1de-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b1de-115">Parent elements</span></span>

|<span data-ttu-id="9b1de-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b1de-116">**Element**</span></span>|<span data-ttu-id="9b1de-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b1de-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b1de-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="9b1de-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="9b1de-119">Représente un abonnement à un abonnement de notification push d’événements.</span><span class="sxs-lookup"><span data-stu-id="9b1de-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b1de-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9b1de-120">Text value</span></span>

<span data-ttu-id="9b1de-121">Une valeur de texte qui représente un entier est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="9b1de-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="9b1de-122">Les valeurs possibles de cet élément sont 1 et 1440 (inclus).</span><span class="sxs-lookup"><span data-stu-id="9b1de-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="9b1de-123">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9b1de-123">This element is optional.</span></span> <span data-ttu-id="9b1de-124">La valeur par défaut est 30 minutes.</span><span class="sxs-lookup"><span data-stu-id="9b1de-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b1de-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="9b1de-125">Remarks</span></span>

<span data-ttu-id="9b1de-126">La valeur de **StatusFrequency** est utilisée par le serveur pour réessayer une notification push lorsqu’il ne reçoit pas une réponse à une notification push ou un état ping à partir du client.</span><span class="sxs-lookup"><span data-stu-id="9b1de-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="9b1de-127">Si le serveur ne reçoit pas de réponse, il réessayer d’envoyer la notification plusieurs fois avant qu’elle cesse d’envoyer la notification.</span><span class="sxs-lookup"><span data-stu-id="9b1de-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="9b1de-128">Dans les services EWS, l’intervalle entre tentatives par défaut est de 30 secondes et tentatives suivantes sont toujours double l’heure de la dernière période de nouvelle tentative.</span><span class="sxs-lookup"><span data-stu-id="9b1de-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="9b1de-129">Temps de nouvelle tentative ne sont pas exactes comme ils peuvent être retardées en raison d’autres charges sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="9b1de-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="9b1de-130">Le tableau suivant indique comment les intervalles se produisent dans les 30 minutes alloués à la valeur de **StatusFrequency** par défaut (en supposant que le serveur n’a pas trouvé les retards).</span><span class="sxs-lookup"><span data-stu-id="9b1de-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="9b1de-131">**Réessayer**</span><span class="sxs-lookup"><span data-stu-id="9b1de-131">**Retry**</span></span>|<span data-ttu-id="9b1de-132">**Secondes**</span><span class="sxs-lookup"><span data-stu-id="9b1de-132">**Seconds**</span></span>|<span data-ttu-id="9b1de-133">**Heure**</span><span class="sxs-lookup"><span data-stu-id="9b1de-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9b1de-134">0</span><span class="sxs-lookup"><span data-stu-id="9b1de-134">0</span></span>  <br/> |<span data-ttu-id="9b1de-135">0</span><span class="sxs-lookup"><span data-stu-id="9b1de-135">0</span></span>  <br/> |<span data-ttu-id="9b1de-136">Synchronisation initiale</span><span class="sxs-lookup"><span data-stu-id="9b1de-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="9b1de-137">1</span><span class="sxs-lookup"><span data-stu-id="9b1de-137">1</span></span>  <br/> |<span data-ttu-id="9b1de-138">30</span><span class="sxs-lookup"><span data-stu-id="9b1de-138">30</span></span>  <br/> |<span data-ttu-id="9b1de-139">00:30</span><span class="sxs-lookup"><span data-stu-id="9b1de-139">00:30</span></span>  <br/> |
|<span data-ttu-id="9b1de-140">2</span><span class="sxs-lookup"><span data-stu-id="9b1de-140">2</span></span>  <br/> |<span data-ttu-id="9b1de-141">60</span><span class="sxs-lookup"><span data-stu-id="9b1de-141">60</span></span>  <br/> |<span data-ttu-id="9b1de-142">01:00</span><span class="sxs-lookup"><span data-stu-id="9b1de-142">01:00</span></span>  <br/> |
|<span data-ttu-id="9b1de-143">3</span><span class="sxs-lookup"><span data-stu-id="9b1de-143">3</span></span>  <br/> |<span data-ttu-id="9b1de-144">120</span><span class="sxs-lookup"><span data-stu-id="9b1de-144">120</span></span>  <br/> |<span data-ttu-id="9b1de-145">02:00</span><span class="sxs-lookup"><span data-stu-id="9b1de-145">02:00</span></span>  <br/> |
|<span data-ttu-id="9b1de-146">4</span><span class="sxs-lookup"><span data-stu-id="9b1de-146">4</span></span>  <br/> |<span data-ttu-id="9b1de-147">240</span><span class="sxs-lookup"><span data-stu-id="9b1de-147">240</span></span>  <br/> |<span data-ttu-id="9b1de-148">04:00</span><span class="sxs-lookup"><span data-stu-id="9b1de-148">04:00</span></span>  <br/> |
|<span data-ttu-id="9b1de-149">5</span><span class="sxs-lookup"><span data-stu-id="9b1de-149">5</span></span>  <br/> |<span data-ttu-id="9b1de-150">480</span><span class="sxs-lookup"><span data-stu-id="9b1de-150">480</span></span>  <br/> |<span data-ttu-id="9b1de-151">08:00</span><span class="sxs-lookup"><span data-stu-id="9b1de-151">08:00</span></span>  <br/> |
|<span data-ttu-id="9b1de-152">6</span><span class="sxs-lookup"><span data-stu-id="9b1de-152">6</span></span>  <br/> |<span data-ttu-id="9b1de-153">960</span><span class="sxs-lookup"><span data-stu-id="9b1de-153">960</span></span>  <br/> |<span data-ttu-id="9b1de-154">16:00</span><span class="sxs-lookup"><span data-stu-id="9b1de-154">16:00</span></span>  <br/> |
|<span data-ttu-id="9b1de-155">7</span><span class="sxs-lookup"><span data-stu-id="9b1de-155">7</span></span>  <br/> |<span data-ttu-id="9b1de-156">1920</span><span class="sxs-lookup"><span data-stu-id="9b1de-156">1920</span></span>  <br/> |<span data-ttu-id="9b1de-157">32:00 - valeur par défaut **StatusFrequency** 30 dépassé, nouvelle tentative ne pas envoyé</span><span class="sxs-lookup"><span data-stu-id="9b1de-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="9b1de-158">Si le client ne reçoit pas les messages de notification à partir du serveur pour une période de temps qui dépasse deux fois la durée spécifiée par **StatusFrequency**, le client doit effectuer une action tels que recréer l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="9b1de-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="9b1de-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b1de-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b1de-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b1de-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b1de-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b1de-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b1de-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b1de-162">Schema name</span></span>  <br/> |<span data-ttu-id="9b1de-163">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9b1de-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b1de-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9b1de-164">Validation file</span></span>  <br/> |<span data-ttu-id="9b1de-165">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9b1de-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b1de-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b1de-166">Can be empty</span></span>  <br/> |<span data-ttu-id="9b1de-167">False</span><span class="sxs-lookup"><span data-stu-id="9b1de-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b1de-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b1de-168">See also</span></span>



[<span data-ttu-id="9b1de-169">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="9b1de-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="9b1de-170">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="9b1de-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="9b1de-171">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="9b1de-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="9b1de-172">Filigrane</span><span class="sxs-lookup"><span data-stu-id="9b1de-172">Watermark</span></span>](watermark.md)

