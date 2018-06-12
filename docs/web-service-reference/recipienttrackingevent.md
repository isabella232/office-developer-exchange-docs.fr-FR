---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: L’élément RecipientTrackingEvent contient des informations pour un seul événement pour un destinataire.
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828989"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="c3643-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="c3643-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="c3643-104">L’élément **RecipientTrackingEvent** contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="c3643-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 <span data-ttu-id="c3643-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="c3643-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3643-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c3643-106">Attributes and elements</span></span>

<span data-ttu-id="c3643-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c3643-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3643-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c3643-108">Attributes</span></span>

<span data-ttu-id="c3643-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c3643-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3643-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c3643-110">Child elements</span></span>

|<span data-ttu-id="c3643-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c3643-111">**Element**</span></span>|<span data-ttu-id="c3643-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c3643-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3643-113">Date (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="c3643-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="c3643-114">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-115">Recipient</span><span class="sxs-lookup"><span data-stu-id="c3643-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="c3643-116">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="c3643-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="c3643-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-119">EventDescription</span><span class="sxs-lookup"><span data-stu-id="c3643-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="c3643-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-121">EventData</span><span class="sxs-lookup"><span data-stu-id="c3643-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="c3643-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c3643-123">Serveur (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="c3643-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="c3643-124">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="c3643-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="c3643-126">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c3643-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c3643-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="c3643-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="c3643-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c3643-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="c3643-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="c3643-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c3643-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="c3643-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="c3643-132">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c3643-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="c3643-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="c3643-134">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c3643-135">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="c3643-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="c3643-136">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c3643-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c3643-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c3643-137">Parent elements</span></span>

|<span data-ttu-id="c3643-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c3643-138">**Element**</span></span>|<span data-ttu-id="c3643-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="c3643-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3643-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="c3643-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="c3643-141">Contient une liste d’un ou plusieurs événements de suivi pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="c3643-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3643-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c3643-142">Text value</span></span>

<span data-ttu-id="c3643-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c3643-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3643-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="c3643-144">Remarks</span></span>

<span data-ttu-id="c3643-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3643-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3643-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c3643-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3643-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c3643-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3643-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c3643-148">Schema Name</span></span>  <br/> |<span data-ttu-id="c3643-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c3643-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="c3643-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c3643-150">Validation File</span></span>  <br/> |<span data-ttu-id="c3643-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c3643-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3643-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c3643-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="c3643-153">False</span><span class="sxs-lookup"><span data-stu-id="c3643-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c3643-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c3643-154">See also</span></span>



[<span data-ttu-id="c3643-155">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c3643-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="c3643-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c3643-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
