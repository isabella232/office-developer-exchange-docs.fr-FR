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
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465484"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="542c6-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="542c6-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="542c6-104">L’élément **RecipientTrackingEvent** contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="542c6-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
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

 <span data-ttu-id="542c6-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="542c6-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="542c6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="542c6-106">Attributes and elements</span></span>

<span data-ttu-id="542c6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="542c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="542c6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="542c6-108">Attributes</span></span>

<span data-ttu-id="542c6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="542c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="542c6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="542c6-110">Child elements</span></span>

|<span data-ttu-id="542c6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="542c6-111">**Element**</span></span>|<span data-ttu-id="542c6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="542c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="542c6-113">Date (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="542c6-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="542c6-114">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-115">Destinataire</span><span class="sxs-lookup"><span data-stu-id="542c6-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="542c6-116">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="542c6-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="542c6-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-119">Systèmedescription</span><span class="sxs-lookup"><span data-stu-id="542c6-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="542c6-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-121">EventData</span><span class="sxs-lookup"><span data-stu-id="542c6-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="542c6-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="542c6-123">Serveur (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="542c6-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="542c6-124">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="542c6-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="542c6-126">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="542c6-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="542c6-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="542c6-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="542c6-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="542c6-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="542c6-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="542c6-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="542c6-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="542c6-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="542c6-132">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="542c6-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="542c6-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="542c6-134">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="542c6-135">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="542c6-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="542c6-136">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="542c6-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="542c6-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="542c6-137">Parent elements</span></span>

|<span data-ttu-id="542c6-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="542c6-138">**Element**</span></span>|<span data-ttu-id="542c6-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="542c6-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="542c6-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="542c6-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="542c6-141">Contient une liste d’un ou plusieurs événements de suivi pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="542c6-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="542c6-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="542c6-142">Text value</span></span>

<span data-ttu-id="542c6-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="542c6-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="542c6-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="542c6-144">Remarks</span></span>

<span data-ttu-id="542c6-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="542c6-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="542c6-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="542c6-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="542c6-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="542c6-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="542c6-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="542c6-148">Schema Name</span></span>  <br/> |<span data-ttu-id="542c6-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="542c6-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="542c6-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="542c6-150">Validation File</span></span>  <br/> |<span data-ttu-id="542c6-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="542c6-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="542c6-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="542c6-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="542c6-153">False</span><span class="sxs-lookup"><span data-stu-id="542c6-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="542c6-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="542c6-154">See also</span></span>



[<span data-ttu-id="542c6-155">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="542c6-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="542c6-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="542c6-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

