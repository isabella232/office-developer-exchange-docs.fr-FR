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
description: L’élément PushSubscriptionRequest représente un abonnement à un abonnement de notification d’événement basé sur un type de message.
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465512"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="fe7e6-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="fe7e6-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="fe7e6-104">L’élément **PushSubscriptionRequest** représente un abonnement à un abonnement de notification d’événement basé sur un type de message.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="fe7e6-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="fe7e6-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="fe7e6-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="fe7e6-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="fe7e6-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe7e6-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe7e6-108">Attributes and elements</span></span>

<span data-ttu-id="fe7e6-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe7e6-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe7e6-110">Attributes</span></span>

|<span data-ttu-id="fe7e6-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-111">**Attribute**</span></span>|<span data-ttu-id="fe7e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe7e6-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="fe7e6-114">Indique s’il faut s’abonner à tous les dossiers disponibles.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="fe7e6-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fe7e6-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe7e6-116">Child elements</span></span>

|<span data-ttu-id="fe7e6-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-117">**Element**</span></span>|<span data-ttu-id="fe7e6-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe7e6-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="fe7e6-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="fe7e6-120">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à surveiller pour les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="fe7e6-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="fe7e6-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="fe7e6-122">Contient une collection de notifications d’événements qui sont utilisées pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="fe7e6-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="fe7e6-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="fe7e6-124">Représente un signet d’événement dans la table des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="fe7e6-125">Cela permet de créer un abonnement à partir d’un événement représenté par le filigrane.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="fe7e6-126">Si le filigrane d’une demande subscribe est introuvable, une réponse d’erreur est renvoyée au client.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="fe7e6-127">Cela peut se produire si le filigrane est âgé de plus de 30 jours ou si le filigrane n’a jamais été présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fe7e6-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="fe7e6-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="fe7e6-129">Représente la fréquence, spécifiée en minutes, à laquelle les messages de notification sont envoyés au client lorsqu’aucun événement n’a eu lieu.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="fe7e6-130">Adresse</span><span class="sxs-lookup"><span data-stu-id="fe7e6-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fe7e6-131">Représente l’emplacement du service Web client pour les notifications de type transmission.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe7e6-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe7e6-132">Parent elements</span></span>

|<span data-ttu-id="fe7e6-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-133">**Element**</span></span>|<span data-ttu-id="fe7e6-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe7e6-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe7e6-135">S’abonner</span><span class="sxs-lookup"><span data-stu-id="fe7e6-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="fe7e6-136">Contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe7e6-137">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fe7e6-137">Text value</span></span>

<span data-ttu-id="fe7e6-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fe7e6-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe7e6-139">Remarks</span></span>

<span data-ttu-id="fe7e6-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe7e6-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe7e6-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe7e6-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe7e6-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe7e6-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fe7e6-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe7e6-143">Schema name</span></span>  <br/> |<span data-ttu-id="fe7e6-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fe7e6-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fe7e6-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe7e6-145">Validation file</span></span>  <br/> |<span data-ttu-id="fe7e6-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fe7e6-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe7e6-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe7e6-147">Can be empty</span></span>  <br/> |<span data-ttu-id="fe7e6-148">False</span><span class="sxs-lookup"><span data-stu-id="fe7e6-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe7e6-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe7e6-149">See also</span></span>



[<span data-ttu-id="fe7e6-150">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="fe7e6-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="fe7e6-151">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="fe7e6-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="fe7e6-152">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="fe7e6-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

