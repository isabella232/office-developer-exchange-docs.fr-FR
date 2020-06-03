---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: L’élément Watermark représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres.
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459762"
---
# <a name="watermark"></a><span data-ttu-id="db09d-103">Watermark</span><span class="sxs-lookup"><span data-stu-id="db09d-103">Watermark</span></span>

<span data-ttu-id="db09d-104">L’élément **Watermark** représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db09d-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="db09d-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="db09d-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db09d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="db09d-106">Attributes and elements</span></span>

<span data-ttu-id="db09d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="db09d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db09d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="db09d-108">Attributes</span></span>

<span data-ttu-id="db09d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="db09d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db09d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="db09d-110">Child elements</span></span>

<span data-ttu-id="db09d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="db09d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db09d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="db09d-112">Parent elements</span></span>

|<span data-ttu-id="db09d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="db09d-113">**Element**</span></span>|<span data-ttu-id="db09d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="db09d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db09d-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="db09d-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="db09d-116">Représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.</span><span class="sxs-lookup"><span data-stu-id="db09d-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="db09d-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="db09d-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="db09d-118">Représente un abonnement à un abonnement de notification d’événement basé sur un type de message.</span><span class="sxs-lookup"><span data-stu-id="db09d-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="db09d-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="db09d-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="db09d-120">Représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="db09d-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="db09d-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="db09d-122">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="db09d-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="db09d-123">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="db09d-124">Représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="db09d-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="db09d-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="db09d-126">Représente un événement dans lequel un élément ou un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="db09d-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="db09d-127">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="db09d-128">Représente un événement dans lequel un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="db09d-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="db09d-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="db09d-130">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="db09d-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="db09d-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="db09d-132">Représente un événement déclenché par un nouvel élément de courrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db09d-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="db09d-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="db09d-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="db09d-134">Représente une notification indiquant qu’aucune nouvelle activité n’a eu lieu dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db09d-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="db09d-135">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="db09d-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="db09d-136">Contient l’État et le résultat d’une demande subscribe.</span><span class="sxs-lookup"><span data-stu-id="db09d-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db09d-137">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="db09d-137">Text value</span></span>

<span data-ttu-id="db09d-138">Une valeur de texte peut être obligatoire ou facultative en fonction de la façon dont cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="db09d-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db09d-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="db09d-139">Remarks</span></span>

<span data-ttu-id="db09d-140">Si une demande subscribe contient un filigrane, l’abonnement est créé à partir du filigrane avant.</span><span class="sxs-lookup"><span data-stu-id="db09d-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="db09d-141">Si la demande subscribe contient un filigrane qui est introuvable dans la table des événements de boîte aux lettres, une `ErrorInvalidWatermark` erreur est renvoyée à l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="db09d-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="db09d-142">Cela peut se produire si le filigrane est trop ancien et a été supprimé de la fenêtre de 30 jours de la table des événements ou si le filigrane n’était jamais présent dans la table des événements.</span><span class="sxs-lookup"><span data-stu-id="db09d-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="db09d-143">Cela peut se produire, par exemple, si un filigrane est obtenu à partir d’un autre abonnement pour une boîte aux lettres dans une autre base de données.</span><span class="sxs-lookup"><span data-stu-id="db09d-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="db09d-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="db09d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db09d-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="db09d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db09d-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="db09d-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db09d-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="db09d-147">Schema name</span></span>  <br/> |<span data-ttu-id="db09d-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="db09d-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="db09d-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="db09d-149">Validation file</span></span>  <br/> |<span data-ttu-id="db09d-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db09d-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db09d-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="db09d-151">Can be empty</span></span>  <br/> |<span data-ttu-id="db09d-152">False</span><span class="sxs-lookup"><span data-stu-id="db09d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db09d-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="db09d-153">See also</span></span>



[<span data-ttu-id="db09d-154">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="db09d-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="db09d-155">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="db09d-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="db09d-156">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="db09d-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)

