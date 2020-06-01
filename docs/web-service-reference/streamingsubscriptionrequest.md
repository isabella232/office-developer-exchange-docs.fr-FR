---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: L’élément StreamingSubscriptionRequest représente un abonnement à un abonnement de notification d’événements en continu.
ms.openlocfilehash: b469ba7598420189c1db0e2fe676a279390eb6bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468228"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="39719-103">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="39719-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="39719-104">L’élément **StreamingSubscriptionRequest** représente un abonnement à un abonnement de notification d’événements en continu.</span><span class="sxs-lookup"><span data-stu-id="39719-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="39719-105">S’abonner</span><span class="sxs-lookup"><span data-stu-id="39719-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="39719-106">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="39719-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="39719-107">**StreamingSubscriptionRequest**</span><span class="sxs-lookup"><span data-stu-id="39719-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39719-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="39719-108">Attributes and elements</span></span>

<span data-ttu-id="39719-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="39719-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39719-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="39719-110">Attributes</span></span>

|<span data-ttu-id="39719-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="39719-111">**Attribute**</span></span>|<span data-ttu-id="39719-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="39719-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39719-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="39719-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="39719-114">Indique si le serveur doit s’abonner à tous les dossiers de la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="39719-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="39719-115">La valeur **true** indique que le serveur s’abonne.</span><span class="sxs-lookup"><span data-stu-id="39719-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="39719-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="39719-116">Child elements</span></span>

|<span data-ttu-id="39719-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="39719-117">**Element**</span></span>|<span data-ttu-id="39719-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="39719-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39719-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="39719-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="39719-120">Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à surveiller pour les notifications d’événement.</span><span class="sxs-lookup"><span data-stu-id="39719-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="39719-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="39719-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="39719-122">Contient une collection de notifications d’événements qui sont utilisées pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="39719-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39719-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="39719-123">Parent elements</span></span>

|<span data-ttu-id="39719-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="39719-124">**Element**</span></span>|<span data-ttu-id="39719-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="39719-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39719-126">S’abonner</span><span class="sxs-lookup"><span data-stu-id="39719-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="39719-127">Contient les propriétés utilisées pour créer des abonnements.</span><span class="sxs-lookup"><span data-stu-id="39719-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="39719-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="39719-128">Text value</span></span>

<span data-ttu-id="39719-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="39719-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39719-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="39719-130">Remarks</span></span>

<span data-ttu-id="39719-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="39719-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39719-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="39719-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39719-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="39719-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39719-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="39719-134">Schema name</span></span>  <br/> |<span data-ttu-id="39719-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="39719-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39719-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="39719-136">Validation file</span></span>  <br/> |<span data-ttu-id="39719-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="39719-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39719-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="39719-138">Can be empty</span></span>  <br/> |<span data-ttu-id="39719-139">False</span><span class="sxs-lookup"><span data-stu-id="39719-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39719-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="39719-140">See also</span></span>



[<span data-ttu-id="39719-141">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="39719-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="39719-142">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="39719-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="39719-143">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="39719-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="39719-144">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="39719-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

