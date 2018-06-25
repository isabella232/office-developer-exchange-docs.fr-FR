---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: L’élément PullSubscriptionRequest représente un abonnement à un abonnement de notification d’événement de type pull.
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828932"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="4a1c3-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="4a1c3-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="4a1c3-104">L’élément **PullSubscriptionRequest** représente un abonnement à un abonnement de notification d’événement de type pull.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="4a1c3-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="4a1c3-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="4a1c3-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="4a1c3-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="4a1c3-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a1c3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a1c3-108">Attributes and elements</span></span>

<span data-ttu-id="4a1c3-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a1c3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a1c3-110">Attributes</span></span>

|<span data-ttu-id="4a1c3-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-111">**Attribute**</span></span>|<span data-ttu-id="4a1c3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a1c3-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="4a1c3-114">Indique s’il s’abonner à tous les dossiers disponibles.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="4a1c3-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4a1c3-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a1c3-116">Child elements</span></span>

|<span data-ttu-id="4a1c3-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-117">**Element**</span></span>|<span data-ttu-id="4a1c3-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a1c3-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="4a1c3-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="4a1c3-120">Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à analyser pour les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="4a1c3-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="4a1c3-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="4a1c3-122">Contient une collection de notifications d’événements qui sont utilisés pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="4a1c3-123">Filigrane</span><span class="sxs-lookup"><span data-stu-id="4a1c3-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="4a1c3-124">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="4a1c3-125">Cela permet de créer un abonnement démarre à un événement qui est représenté par le filigrane.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="4a1c3-126">Si la limite d’une demande Subscribe n’est trouvée, une réponse d’erreur est retournée au client.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="4a1c3-127">Cette erreur peut se produire si celui-ci est antérieure à 30 jours ou si celui-ci n’a jamais été présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4a1c3-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="4a1c3-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="4a1c3-129">Représente la durée, en minutes, pendant laquelle l’abonnement peut rester inactive sans GetEvents demande à partir du client.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a1c3-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a1c3-130">Parent elements</span></span>

|<span data-ttu-id="4a1c3-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-131">**Element**</span></span>|<span data-ttu-id="4a1c3-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a1c3-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a1c3-133">S’abonner</span><span class="sxs-lookup"><span data-stu-id="4a1c3-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="4a1c3-134">Contient les propriétés qui sont utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a1c3-135">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4a1c3-135">Text value</span></span>

<span data-ttu-id="4a1c3-136">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a1c3-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a1c3-137">Remarks</span></span>

<span data-ttu-id="4a1c3-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a1c3-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a1c3-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a1c3-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a1c3-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a1c3-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a1c3-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a1c3-141">Schema name</span></span>  <br/> |<span data-ttu-id="4a1c3-142">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4a1c3-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4a1c3-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a1c3-143">Validation file</span></span>  <br/> |<span data-ttu-id="4a1c3-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4a1c3-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a1c3-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a1c3-145">Can be empty</span></span>  <br/> |<span data-ttu-id="4a1c3-146">False</span><span class="sxs-lookup"><span data-stu-id="4a1c3-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a1c3-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a1c3-147">See also</span></span>



[<span data-ttu-id="4a1c3-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="4a1c3-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="4a1c3-149">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4a1c3-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="4a1c3-150">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="4a1c3-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="4a1c3-151">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4a1c3-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="4a1c3-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4a1c3-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

