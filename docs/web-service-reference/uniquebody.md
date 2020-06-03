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
description: L’élément UniqueBody représente un fragment HTML ou du texte brut qui représente le corps unique de cette conversation.
ms.openlocfilehash: 0a8d52c7d4eb8bda9fd41c4c25e448523185df93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461918"
---
# <a name="uniquebody"></a><span data-ttu-id="5c5c0-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="5c5c0-103">UniqueBody</span></span>

<span data-ttu-id="5c5c0-104">L’élément **UniqueBody** représente un fragment HTML ou du texte brut qui représente le corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="5c5c0-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c5c0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5c5c0-106">Attributes and elements</span></span>

<span data-ttu-id="5c5c0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c5c0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5c5c0-108">Attributes</span></span>

|<span data-ttu-id="5c5c0-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-109">**Attribute**</span></span>|<span data-ttu-id="5c5c0-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c5c0-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-111">**BodyType**</span></span> <br/> |<span data-ttu-id="5c5c0-112">Indique comment le corps de l’élément est stocké dans l’élément.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="5c5c0-113">Attribut BodyType</span><span class="sxs-lookup"><span data-stu-id="5c5c0-113">BodyType Attribute</span></span>

|<span data-ttu-id="5c5c0-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-114">**Value**</span></span>|<span data-ttu-id="5c5c0-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c5c0-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-116">**HTML**</span></span> <br/> |<span data-ttu-id="5c5c0-117">Convertit tous les corps au format HTML.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="5c5c0-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-118">**Text**</span></span> <br/> |<span data-ttu-id="5c5c0-119">Convertit tous les corps en texte brut.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5c5c0-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5c5c0-120">Child elements</span></span>

<span data-ttu-id="5c5c0-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c5c0-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5c5c0-122">Parent elements</span></span>

|<span data-ttu-id="5c5c0-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-123">**Element**</span></span>|<span data-ttu-id="5c5c0-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c5c0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c5c0-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5c5c0-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5c5c0-126">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-127">Contact</span><span class="sxs-lookup"><span data-stu-id="5c5c0-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5c5c0-128">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="5c5c0-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5c5c0-130">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-131">Élément</span><span class="sxs-lookup"><span data-stu-id="5c5c0-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="5c5c0-132">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5c5c0-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5c5c0-134">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5c5c0-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5c5c0-136">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-137">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="5c5c0-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5c5c0-138">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5c5c0-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5c5c0-140">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-141">Message</span><span class="sxs-lookup"><span data-stu-id="5c5c0-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c5c0-142">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-143">PostItem</span><span class="sxs-lookup"><span data-stu-id="5c5c0-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="5c5c0-144">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="5c5c0-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="5c5c0-146">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c5c0-147">Tâche</span><span class="sxs-lookup"><span data-stu-id="5c5c0-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="5c5c0-148">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c5c0-149">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5c5c0-149">Text value</span></span>

<span data-ttu-id="5c5c0-150">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c5c0-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="5c5c0-151">Remarks</span></span>

<span data-ttu-id="5c5c0-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c5c0-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c5c0-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5c5c0-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c5c0-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5c5c0-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c5c0-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5c5c0-155">Schema Name</span></span>  <br/> |<span data-ttu-id="5c5c0-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5c5c0-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c5c0-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5c5c0-157">Validation File</span></span>  <br/> |<span data-ttu-id="5c5c0-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c5c0-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c5c0-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5c5c0-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c5c0-160">False</span><span class="sxs-lookup"><span data-stu-id="5c5c0-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c5c0-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5c5c0-161">See also</span></span>



- [<span data-ttu-id="5c5c0-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5c5c0-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

