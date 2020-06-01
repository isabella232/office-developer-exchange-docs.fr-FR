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
description: L’élément StatusFrequency représente la valeur de délai d’expiration maximale, en minutes, pendant laquelle les nouvelles tentatives sont tentées par le serveur.
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468242"
---
# <a name="statusfrequency"></a><span data-ttu-id="6b3c4-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="6b3c4-103">StatusFrequency</span></span>

<span data-ttu-id="6b3c4-104">L’élément **StatusFrequency** représente la valeur de délai d’expiration maximale, en minutes, pendant laquelle les nouvelles tentatives sont tentées par le serveur.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="6b3c4-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="6b3c4-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="6b3c4-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="6b3c4-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="6b3c4-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="6b3c4-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="6b3c4-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b3c4-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6b3c4-109">Attributes and elements</span></span>

<span data-ttu-id="6b3c4-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b3c4-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="6b3c4-111">Attributes</span></span>

<span data-ttu-id="6b3c4-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b3c4-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6b3c4-113">Child elements</span></span>

<span data-ttu-id="6b3c4-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b3c4-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6b3c4-115">Parent elements</span></span>

|<span data-ttu-id="6b3c4-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-116">**Element**</span></span>|<span data-ttu-id="6b3c4-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b3c4-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="6b3c4-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="6b3c4-119">Représente un abonnement à un abonnement de notification d’événement basé sur un type de message.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b3c4-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6b3c4-120">Text value</span></span>

<span data-ttu-id="6b3c4-121">Une valeur de texte qui représente un entier est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="6b3c4-122">Les valeurs possibles de cet élément sont comprises entre 1 et 1440 inclus.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="6b3c4-123">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-123">This element is optional.</span></span> <span data-ttu-id="6b3c4-124">La valeur par défaut est 30 minutes.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b3c4-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="6b3c4-125">Remarks</span></span>

<span data-ttu-id="6b3c4-126">La valeur **StatusFrequency** est utilisée par le serveur pour renouveler une notification de transmission lorsqu’il ne reçoit pas de réponse à une notification d’envoi ou à un ping d’État à partir du client.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="6b3c4-127">Si le serveur ne reçoit pas de réponse, il essaie d’envoyer la notification plusieurs fois avant d’arrêter l’envoi de la notification.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="6b3c4-128">Dans EWS, l’intervalle de nouvelle tentative par défaut est de 30 secondes et les tentatives suivantes sont toujours effectuées deux fois l’heure de la dernière tentative.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="6b3c4-129">Les durées de nouvelle tentative ne sont pas exactes car elles peuvent être retardées en raison d’autres charges sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="6b3c4-130">Le tableau suivant indique comment les intervalles de nouvelle tentative se produisent dans les 30 minutes allouées par la valeur **StatusFrequency** par défaut (en supposant que le serveur n’a rencontré aucun retard).</span><span class="sxs-lookup"><span data-stu-id="6b3c4-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="6b3c4-131">**Réessayer**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-131">**Retry**</span></span>|<span data-ttu-id="6b3c4-132">**Secondes**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-132">**Seconds**</span></span>|<span data-ttu-id="6b3c4-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="6b3c4-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b3c4-134">0</span><span class="sxs-lookup"><span data-stu-id="6b3c4-134">0</span></span>  <br/> |<span data-ttu-id="6b3c4-135">0</span><span class="sxs-lookup"><span data-stu-id="6b3c4-135">0</span></span>  <br/> |<span data-ttu-id="6b3c4-136">Synchronisation initiale</span><span class="sxs-lookup"><span data-stu-id="6b3c4-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="6b3c4-137">1 </span><span class="sxs-lookup"><span data-stu-id="6b3c4-137">1</span></span>  <br/> |<span data-ttu-id="6b3c4-138">0,30</span><span class="sxs-lookup"><span data-stu-id="6b3c4-138">30</span></span>  <br/> |<span data-ttu-id="6b3c4-139">00:30</span><span class="sxs-lookup"><span data-stu-id="6b3c4-139">00:30</span></span>  <br/> |
|<span data-ttu-id="6b3c4-140">n°2</span><span class="sxs-lookup"><span data-stu-id="6b3c4-140">2</span></span>  <br/> |<span data-ttu-id="6b3c4-141">60</span><span class="sxs-lookup"><span data-stu-id="6b3c4-141">60</span></span>  <br/> |<span data-ttu-id="6b3c4-142">01:00</span><span class="sxs-lookup"><span data-stu-id="6b3c4-142">01:00</span></span>  <br/> |
|<span data-ttu-id="6b3c4-143">3</span><span class="sxs-lookup"><span data-stu-id="6b3c4-143">3</span></span>  <br/> |<span data-ttu-id="6b3c4-144">120</span><span class="sxs-lookup"><span data-stu-id="6b3c4-144">120</span></span>  <br/> |<span data-ttu-id="6b3c4-145">02:00</span><span class="sxs-lookup"><span data-stu-id="6b3c4-145">02:00</span></span>  <br/> |
|<span data-ttu-id="6b3c4-146">4 </span><span class="sxs-lookup"><span data-stu-id="6b3c4-146">4</span></span>  <br/> |<span data-ttu-id="6b3c4-147">240</span><span class="sxs-lookup"><span data-stu-id="6b3c4-147">240</span></span>  <br/> |<span data-ttu-id="6b3c4-148">04:00</span><span class="sxs-lookup"><span data-stu-id="6b3c4-148">04:00</span></span>  <br/> |
|<span data-ttu-id="6b3c4-149">5 </span><span class="sxs-lookup"><span data-stu-id="6b3c4-149">5</span></span>  <br/> |<span data-ttu-id="6b3c4-150">480</span><span class="sxs-lookup"><span data-stu-id="6b3c4-150">480</span></span>  <br/> |<span data-ttu-id="6b3c4-151">08:00</span><span class="sxs-lookup"><span data-stu-id="6b3c4-151">08:00</span></span>  <br/> |
|<span data-ttu-id="6b3c4-152">6 </span><span class="sxs-lookup"><span data-stu-id="6b3c4-152">6</span></span>  <br/> |<span data-ttu-id="6b3c4-153">960</span><span class="sxs-lookup"><span data-stu-id="6b3c4-153">960</span></span>  <br/> |<span data-ttu-id="6b3c4-154">16:00</span><span class="sxs-lookup"><span data-stu-id="6b3c4-154">16:00</span></span>  <br/> |
|<span data-ttu-id="6b3c4-155">7 </span><span class="sxs-lookup"><span data-stu-id="6b3c4-155">7</span></span>  <br/> |<span data-ttu-id="6b3c4-156">1920</span><span class="sxs-lookup"><span data-stu-id="6b3c4-156">1920</span></span>  <br/> |<span data-ttu-id="6b3c4-157">32:00- **StatusFrequency** valeur par défaut de 30 dépassée, nouvelle tentative non envoyée</span><span class="sxs-lookup"><span data-stu-id="6b3c4-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="6b3c4-158">Si le client ne reçoit pas de messages de notification du serveur pendant une période de temps qui dépasse le double de la durée spécifiée par **StatusFrequency**, le client doit effectuer une action telle que la recréation de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="6b3c4-159">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b3c4-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b3c4-160">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6b3c4-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b3c4-161">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6b3c4-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b3c4-162">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6b3c4-162">Schema name</span></span>  <br/> |<span data-ttu-id="6b3c4-163">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6b3c4-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b3c4-164">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6b3c4-164">Validation file</span></span>  <br/> |<span data-ttu-id="6b3c4-165">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b3c4-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b3c4-166">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6b3c4-166">Can be empty</span></span>  <br/> |<span data-ttu-id="6b3c4-167">False</span><span class="sxs-lookup"><span data-stu-id="6b3c4-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b3c4-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b3c4-168">See also</span></span>



[<span data-ttu-id="6b3c4-169">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="6b3c4-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="6b3c4-170">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="6b3c4-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="6b3c4-171">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="6b3c4-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="6b3c4-172">Watermark</span><span class="sxs-lookup"><span data-stu-id="6b3c4-172">Watermark</span></span>](watermark.md)

