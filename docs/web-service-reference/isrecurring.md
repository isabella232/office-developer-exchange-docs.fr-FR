---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: L’élément IsRecurring indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique. Cet élément est en lecture seule.
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828104"
---
# <a name="isrecurring"></a><span data-ttu-id="0569b-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0569b-104">IsRecurring</span></span>

<span data-ttu-id="0569b-105">L’élément **IsRecurring** indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="0569b-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="0569b-106">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0569b-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="0569b-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0569b-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0569b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0569b-108">Attributes and elements</span></span>

<span data-ttu-id="0569b-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0569b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0569b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0569b-110">Attributes</span></span>

<span data-ttu-id="0569b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0569b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0569b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0569b-112">Child elements</span></span>

<span data-ttu-id="0569b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0569b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0569b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0569b-114">Parent elements</span></span>

|<span data-ttu-id="0569b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0569b-115">**Element**</span></span>|<span data-ttu-id="0569b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="0569b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0569b-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0569b-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0569b-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="0569b-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0569b-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0569b-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0569b-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0569b-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0569b-121">Tâche</span><span class="sxs-lookup"><span data-stu-id="0569b-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="0569b-122">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0569b-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0569b-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0569b-123">Text value</span></span>

<span data-ttu-id="0569b-124">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="0569b-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0569b-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="0569b-125">Remarks</span></span>

<span data-ttu-id="0569b-126">Le tableau suivant montre comment la propriété **IsRecurring** est définie pour les types d’éléments de calendrier différent pour les organisateurs et les participants et pour les demandes de réunion et mises à jour.</span><span class="sxs-lookup"><span data-stu-id="0569b-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="0569b-127">**Type de CalendarItem**</span><span class="sxs-lookup"><span data-stu-id="0569b-127">**CalendarItem Type**</span></span>|<span data-ttu-id="0569b-128">**Organisateur <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="0569b-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="0569b-129">**Attendee <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="0569b-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="0569b-130">**Demande/mise à jour de réunion <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="0569b-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="0569b-131">Occurrence unique</span><span class="sxs-lookup"><span data-stu-id="0569b-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="0569b-132">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="0569b-132">**FALSE**</span></span> <br/> |<span data-ttu-id="0569b-133">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="0569b-133">**FALSE**</span></span> <br/> |<span data-ttu-id="0569b-134">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="0569b-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="0569b-135">Périodique principal</span><span class="sxs-lookup"><span data-stu-id="0569b-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="0569b-136">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="0569b-136">**FALSE**</span></span> <br/> |<span data-ttu-id="0569b-137">**LA VALEUR TRUE**</span><span class="sxs-lookup"><span data-stu-id="0569b-137">**TRUE**</span></span> <br/> |<span data-ttu-id="0569b-138">**LA VALEUR TRUE**</span><span class="sxs-lookup"><span data-stu-id="0569b-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="0569b-139">Exception périodique</span><span class="sxs-lookup"><span data-stu-id="0569b-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="0569b-140">**LA VALEUR TRUE**</span><span class="sxs-lookup"><span data-stu-id="0569b-140">**TRUE**</span></span> <br/> |<span data-ttu-id="0569b-141">**LA VALEUR TRUE**</span><span class="sxs-lookup"><span data-stu-id="0569b-141">**TRUE**</span></span> <br/> |<span data-ttu-id="0569b-142">**LA VALEUR TRUE**</span><span class="sxs-lookup"><span data-stu-id="0569b-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="0569b-143">La valeur de la propriété **IsRecurring** qui est définie pour les éléments périodiques du calendrier principal pour l’organisateur est incorrecte ; Cette valeur doit être définie sur **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="0569b-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0569b-144">L’opération GetUserAvailability a également un élément [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="0569b-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="0569b-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0569b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0569b-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0569b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0569b-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0569b-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0569b-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0569b-148">Schema name</span></span>  <br/> |<span data-ttu-id="0569b-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0569b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="0569b-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0569b-150">Validation file</span></span>  <br/> |<span data-ttu-id="0569b-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0569b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0569b-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0569b-152">Can be empty</span></span>  <br/> |<span data-ttu-id="0569b-153">False</span><span class="sxs-lookup"><span data-stu-id="0569b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0569b-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0569b-154">See also</span></span>



[<span data-ttu-id="0569b-155">TaskType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0569b-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="0569b-156">CalendarEventDetails.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0569b-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="0569b-157">CalendarItemType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0569b-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="0569b-158">MeetingRequestMessageType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0569b-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="0569b-159">CalendarItemType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="0569b-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="0569b-160">MeetingRequestMessageType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="0569b-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="0569b-161">TaskType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="0569b-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="0569b-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0569b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

