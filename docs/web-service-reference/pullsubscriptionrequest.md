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
description: L’élément PullSubscriptionRequest représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.
ms.openlocfilehash: fb9712c9e1481678c2821ee344052783d5c25bf9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468865"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="0f801-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="0f801-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="0f801-104">L’élément **PullSubscriptionRequest** représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.</span><span class="sxs-lookup"><span data-stu-id="0f801-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="0f801-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="0f801-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="0f801-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="0f801-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="0f801-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="0f801-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f801-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f801-108">Attributes and elements</span></span>

<span data-ttu-id="0f801-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f801-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f801-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f801-110">Attributes</span></span>

|<span data-ttu-id="0f801-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0f801-111">**Attribute**</span></span>|<span data-ttu-id="0f801-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f801-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0f801-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="0f801-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="0f801-114">Indique s’il faut s’abonner à tous les dossiers disponibles.</span><span class="sxs-lookup"><span data-stu-id="0f801-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="0f801-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="0f801-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0f801-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f801-116">Child elements</span></span>

|<span data-ttu-id="0f801-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f801-117">**Element**</span></span>|<span data-ttu-id="0f801-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f801-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f801-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="0f801-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="0f801-120">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à surveiller pour les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="0f801-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="0f801-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="0f801-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="0f801-122">Contient une collection de notifications d’événements qui sont utilisées pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="0f801-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="0f801-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="0f801-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="0f801-124">Représente un signet d’événement dans la table des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0f801-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="0f801-125">Cette opération permet de créer un abonnement qui commence au niveau d’un événement représenté par le filigrane.</span><span class="sxs-lookup"><span data-stu-id="0f801-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="0f801-126">Si le filigrane d’une demande subscribe est introuvable, une réponse d’erreur est renvoyée au client.</span><span class="sxs-lookup"><span data-stu-id="0f801-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="0f801-127">Cette erreur peut se produire si le filigrane est âgé de plus de 30 jours ou si le filigrane n’a jamais été présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0f801-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0f801-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="0f801-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="0f801-129">Représente la durée, en minutes, pendant laquelle l’abonnement peut rester inactif sans demande GetEvents du client.</span><span class="sxs-lookup"><span data-stu-id="0f801-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f801-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f801-130">Parent elements</span></span>

|<span data-ttu-id="0f801-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f801-131">**Element**</span></span>|<span data-ttu-id="0f801-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f801-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f801-133">S’abonner</span><span class="sxs-lookup"><span data-stu-id="0f801-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="0f801-134">Contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="0f801-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f801-135">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0f801-135">Text value</span></span>

<span data-ttu-id="0f801-136">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0f801-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f801-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f801-137">Remarks</span></span>

<span data-ttu-id="0f801-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f801-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f801-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f801-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f801-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f801-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0f801-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f801-141">Schema name</span></span>  <br/> |<span data-ttu-id="0f801-142">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0f801-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0f801-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f801-143">Validation file</span></span>  <br/> |<span data-ttu-id="0f801-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0f801-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0f801-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f801-145">Can be empty</span></span>  <br/> |<span data-ttu-id="0f801-146">False</span><span class="sxs-lookup"><span data-stu-id="0f801-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f801-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f801-147">See also</span></span>



[<span data-ttu-id="0f801-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="0f801-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="0f801-149">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="0f801-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0f801-150">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="0f801-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="0f801-151">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="0f801-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="0f801-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f801-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

