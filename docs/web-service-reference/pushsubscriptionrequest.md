---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: L’élément PushSubscriptionRequest représente un abonnement à un abonnement de notification push d’événements.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828929"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="1bbe0-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="1bbe0-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="1bbe0-104">L’élément **PushSubscriptionRequest** représente un abonnement à un abonnement de notification push d’événements.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="1bbe0-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="1bbe0-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="1bbe0-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="1bbe0-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="1bbe0-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bbe0-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1bbe0-108">Attributes and elements</span></span>

<span data-ttu-id="1bbe0-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bbe0-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1bbe0-110">Attributes</span></span>

|<span data-ttu-id="1bbe0-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-111">**Attribute**</span></span>|<span data-ttu-id="1bbe0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1bbe0-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="1bbe0-114">Indique s’il s’abonner à tous les dossiers disponibles.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="1bbe0-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1bbe0-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1bbe0-116">Child elements</span></span>

|<span data-ttu-id="1bbe0-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-117">**Element**</span></span>|<span data-ttu-id="1bbe0-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bbe0-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="1bbe0-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="1bbe0-120">Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à analyser pour les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="1bbe0-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="1bbe0-122">Contient une collection de notifications d’événements qui sont utilisés pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-123">Filigrane</span><span class="sxs-lookup"><span data-stu-id="1bbe0-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="1bbe0-124">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="1bbe0-125">Cela permet de créer un abonnement commençant à un événement représenté par le filigrane.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="1bbe0-126">Si la limite d’une demande Subscribe n’est trouvée, une réponse d’erreur est retournée au client.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="1bbe0-127">Cela peut se produire si celui-ci est antérieure à 30 jours ou si celui-ci n’a jamais été présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="1bbe0-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="1bbe0-129">Représente la fréquence, en minutes, à la notification messages sont envoyées au client lorsqu’aucun événement ne se sont produites.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="1bbe0-130">URL</span><span class="sxs-lookup"><span data-stu-id="1bbe0-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1bbe0-131">Représente l’emplacement du client de service Web pour les notifications push.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bbe0-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1bbe0-132">Parent elements</span></span>

|<span data-ttu-id="1bbe0-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-133">**Element**</span></span>|<span data-ttu-id="1bbe0-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bbe0-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bbe0-135">S’abonner</span><span class="sxs-lookup"><span data-stu-id="1bbe0-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="1bbe0-136">Contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1bbe0-137">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1bbe0-137">Text value</span></span>

<span data-ttu-id="1bbe0-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1bbe0-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="1bbe0-139">Remarks</span></span>

<span data-ttu-id="1bbe0-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bbe0-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bbe0-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1bbe0-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bbe0-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1bbe0-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1bbe0-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1bbe0-143">Schema name</span></span>  <br/> |<span data-ttu-id="1bbe0-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1bbe0-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1bbe0-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1bbe0-145">Validation file</span></span>  <br/> |<span data-ttu-id="1bbe0-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1bbe0-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1bbe0-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1bbe0-147">Can be empty</span></span>  <br/> |<span data-ttu-id="1bbe0-148">False</span><span class="sxs-lookup"><span data-stu-id="1bbe0-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bbe0-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1bbe0-149">See also</span></span>



[<span data-ttu-id="1bbe0-150">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="1bbe0-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="1bbe0-151">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="1bbe0-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="1bbe0-152">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="1bbe0-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

