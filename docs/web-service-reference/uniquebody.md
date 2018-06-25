---
title: UniqueBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueBody
api_type:
- schema
ms.assetid: 06bc95d7-121c-433b-bd27-c2b0eb8c011f
description: L’élément UniqueBody représente un fragment HTML ou du texte brut qui représente le corps de cette conversation unique.
ms.openlocfilehash: 49d3607926e0b985074d79cde76cad084f537f01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838813"
---
# <a name="uniquebody"></a><span data-ttu-id="9c64b-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="9c64b-103">UniqueBody</span></span>

<span data-ttu-id="9c64b-104">L’élément **UniqueBody** représente un fragment HTML ou du texte brut qui représente le corps de cette conversation unique.</span><span class="sxs-lookup"><span data-stu-id="9c64b-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="9c64b-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="9c64b-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c64b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9c64b-106">Attributes and elements</span></span>

<span data-ttu-id="9c64b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9c64b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c64b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9c64b-108">Attributes</span></span>

|<span data-ttu-id="9c64b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9c64b-109">**Attribute**</span></span>|<span data-ttu-id="9c64b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c64b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c64b-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="9c64b-111">**BodyType**</span></span> <br/> |<span data-ttu-id="9c64b-112">Décrit la façon dont le corps de l’élément est stocké dans l’élément.</span><span class="sxs-lookup"><span data-stu-id="9c64b-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="9c64b-113">Attribut BodyType</span><span class="sxs-lookup"><span data-stu-id="9c64b-113">BodyType Attribute</span></span>

|<span data-ttu-id="9c64b-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9c64b-114">**Value**</span></span>|<span data-ttu-id="9c64b-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c64b-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c64b-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="9c64b-116">**HTML**</span></span> <br/> |<span data-ttu-id="9c64b-117">Convertit tous les corps au format HTML.</span><span class="sxs-lookup"><span data-stu-id="9c64b-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="9c64b-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="9c64b-118">**Text**</span></span> <br/> |<span data-ttu-id="9c64b-119">Convertit tous les corps de texte brut.</span><span class="sxs-lookup"><span data-stu-id="9c64b-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9c64b-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9c64b-120">Child elements</span></span>

<span data-ttu-id="9c64b-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9c64b-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c64b-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9c64b-122">Parent elements</span></span>

|<span data-ttu-id="9c64b-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c64b-123">**Element**</span></span>|<span data-ttu-id="9c64b-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c64b-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c64b-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9c64b-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9c64b-126">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-127">Contact</span><span class="sxs-lookup"><span data-stu-id="9c64b-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9c64b-128">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9c64b-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="9c64b-130">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9c64b-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-131">Élément</span><span class="sxs-lookup"><span data-stu-id="9c64b-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="9c64b-132">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9c64b-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9c64b-134">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9c64b-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9c64b-136">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9c64b-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9c64b-138">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9c64b-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9c64b-140">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-141">Message</span><span class="sxs-lookup"><span data-stu-id="9c64b-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9c64b-142">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-143">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="9c64b-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="9c64b-144">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9c64b-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9c64b-146">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9c64b-147">Tâche</span><span class="sxs-lookup"><span data-stu-id="9c64b-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="9c64b-148">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c64b-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9c64b-149">Text value</span></span>

<span data-ttu-id="9c64b-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9c64b-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c64b-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="9c64b-151">Remarks</span></span>

<span data-ttu-id="9c64b-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c64b-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c64b-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9c64b-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c64b-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9c64b-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c64b-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9c64b-155">Schema Name</span></span>  <br/> |<span data-ttu-id="9c64b-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9c64b-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c64b-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9c64b-157">Validation File</span></span>  <br/> |<span data-ttu-id="9c64b-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c64b-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c64b-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9c64b-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c64b-160">False</span><span class="sxs-lookup"><span data-stu-id="9c64b-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c64b-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9c64b-161">See also</span></span>



- [<span data-ttu-id="9c64b-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9c64b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

