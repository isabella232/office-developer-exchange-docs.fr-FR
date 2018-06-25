---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: L’élément EventType est utilisé pour créer un abonnement et identifie le type d’événement dans une notification.
ms.openlocfilehash: fb54c9e042f105d10e68cb0e9b48feae7ed8bf7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756220"
---
# <a name="eventtype"></a><span data-ttu-id="10122-103">EventType</span><span class="sxs-lookup"><span data-stu-id="10122-103">EventType</span></span>

<span data-ttu-id="10122-104">L’élément **EventType** est utilisé pour créer un abonnement et identifie le type d’événement dans une notification.</span><span class="sxs-lookup"><span data-stu-id="10122-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="10122-105">**NotificationEventTypeType**</span><span class="sxs-lookup"><span data-stu-id="10122-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10122-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="10122-106">Attributes and elements</span></span>

<span data-ttu-id="10122-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="10122-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10122-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="10122-108">Attributes</span></span>

<span data-ttu-id="10122-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10122-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10122-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="10122-110">Child elements</span></span>

<span data-ttu-id="10122-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10122-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10122-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="10122-112">Parent elements</span></span>

|<span data-ttu-id="10122-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10122-113">**Element**</span></span>|<span data-ttu-id="10122-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="10122-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10122-115">EventTypes</span><span class="sxs-lookup"><span data-stu-id="10122-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="10122-116">Contient une collection des types d’événements de notification événement qui sont utilisés pour créer un abonnement.</span><span class="sxs-lookup"><span data-stu-id="10122-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10122-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="10122-117">Text value</span></span>

<span data-ttu-id="10122-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="10122-118">A text value is required.</span></span> <span data-ttu-id="10122-119">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="10122-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="10122-120">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-120">CopiedEvent</span></span>
    
- <span data-ttu-id="10122-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-121">CreatedEvent</span></span>
    
- <span data-ttu-id="10122-122">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-122">DeletedEvent</span></span>
    
- <span data-ttu-id="10122-123">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="10122-124">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-124">MovedEvent</span></span>
    
- <span data-ttu-id="10122-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="10122-125">NewMailEvent</span></span>
    
- <span data-ttu-id="10122-126">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="10122-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="10122-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="10122-127">Remarks</span></span>

<span data-ttu-id="10122-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="10122-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10122-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="10122-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10122-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="10122-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10122-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="10122-131">Schema Name</span></span>  <br/> |<span data-ttu-id="10122-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="10122-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="10122-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="10122-133">Validation File</span></span>  <br/> |<span data-ttu-id="10122-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10122-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10122-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="10122-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="10122-136">False</span><span class="sxs-lookup"><span data-stu-id="10122-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10122-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10122-137">See also</span></span>



[<span data-ttu-id="10122-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="10122-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="10122-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="10122-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="10122-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="10122-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

