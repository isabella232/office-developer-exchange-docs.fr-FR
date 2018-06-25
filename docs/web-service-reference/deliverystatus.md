---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: L’élément DeliveryStatus Spécifie l’état d’un message.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755890"
---
# <a name="deliverystatus"></a><span data-ttu-id="5cf14-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="5cf14-103">DeliveryStatus</span></span>

<span data-ttu-id="5cf14-104">L’élément **DeliveryStatus** Spécifie l’état d’un message.</span><span class="sxs-lookup"><span data-stu-id="5cf14-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="5cf14-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="5cf14-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cf14-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5cf14-106">Attributes and elements</span></span>

<span data-ttu-id="5cf14-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5cf14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cf14-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5cf14-108">Attributes</span></span>

<span data-ttu-id="5cf14-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5cf14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cf14-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5cf14-110">Child elements</span></span>

<span data-ttu-id="5cf14-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5cf14-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5cf14-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5cf14-112">Parent elements</span></span>

|<span data-ttu-id="5cf14-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5cf14-113">**Element**</span></span>|<span data-ttu-id="5cf14-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5cf14-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cf14-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="5cf14-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="5cf14-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="5cf14-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cf14-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5cf14-117">Text value</span></span>

<span data-ttu-id="5cf14-118">Le tableau suivant répertorie les valeurs de texte possibles pour l’élément **DeliveryStatus** .</span><span class="sxs-lookup"><span data-stu-id="5cf14-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="5cf14-119">**Valeurs des éléments DeliveryStatus**</span><span class="sxs-lookup"><span data-stu-id="5cf14-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="5cf14-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5cf14-120">**Value**</span></span>|<span data-ttu-id="5cf14-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="5cf14-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5cf14-122">Échec</span><span class="sxs-lookup"><span data-stu-id="5cf14-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="5cf14-123">Spécifie qu’un message n’a pas été remis.</span><span class="sxs-lookup"><span data-stu-id="5cf14-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="5cf14-124">En attente</span><span class="sxs-lookup"><span data-stu-id="5cf14-124">Pending</span></span>  <br/> |<span data-ttu-id="5cf14-125">Spécifie que le message est en attente d’approbation d’un modérateur.</span><span class="sxs-lookup"><span data-stu-id="5cf14-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="5cf14-126">Remis</span><span class="sxs-lookup"><span data-stu-id="5cf14-126">Delivered</span></span>  <br/> |<span data-ttu-id="5cf14-127">Spécifie que le message a été remis à tous les destinataires spécifiés.</span><span class="sxs-lookup"><span data-stu-id="5cf14-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="5cf14-128">Transféré</span><span class="sxs-lookup"><span data-stu-id="5cf14-128">Transferred</span></span>  <br/> |<span data-ttu-id="5cf14-129">Spécifie que le message a été transféré vers un serveur à l’extérieur de l’étendue de recherche.</span><span class="sxs-lookup"><span data-stu-id="5cf14-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="5cf14-130">Lire</span><span class="sxs-lookup"><span data-stu-id="5cf14-130">Read</span></span>  <br/> |<span data-ttu-id="5cf14-131">Spécifie que le message a été remis et lu par les destinataires.</span><span class="sxs-lookup"><span data-stu-id="5cf14-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5cf14-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="5cf14-132">Remarks</span></span>

<span data-ttu-id="5cf14-133">L’élément **DeliveryStatus** est du type **MessageTrackingDeliveryStatusType** dans Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="5cf14-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="5cf14-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cf14-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cf14-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5cf14-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cf14-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5cf14-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cf14-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5cf14-137">Schema Name</span></span>  <br/> |<span data-ttu-id="5cf14-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5cf14-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="5cf14-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5cf14-139">Validation File</span></span>  <br/> |<span data-ttu-id="5cf14-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cf14-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cf14-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5cf14-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cf14-142">False</span><span class="sxs-lookup"><span data-stu-id="5cf14-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cf14-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5cf14-143">See also</span></span>

- [<span data-ttu-id="5cf14-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5cf14-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

