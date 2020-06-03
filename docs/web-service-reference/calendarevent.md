---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: L’élément CalendarEvent représente une occurrence d’élément de calendrier unique.
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459075"
---
# <a name="calendarevent"></a><span data-ttu-id="0f562-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0f562-103">CalendarEvent</span></span>

<span data-ttu-id="0f562-104">L’élément **CalendarEvent** représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="0f562-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="0f562-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0f562-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0f562-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0f562-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="0f562-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="0f562-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="0f562-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="0f562-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="0f562-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="0f562-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="0f562-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0f562-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="0f562-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="0f562-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f562-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f562-112">Attributes and elements</span></span>

<span data-ttu-id="0f562-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f562-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f562-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f562-114">Attributes</span></span>

<span data-ttu-id="0f562-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0f562-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f562-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f562-116">Child elements</span></span>

|<span data-ttu-id="0f562-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f562-117">**Element**</span></span>|<span data-ttu-id="0f562-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f562-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f562-119">StartTime</span><span class="sxs-lookup"><span data-stu-id="0f562-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="0f562-120">Représente le début d’un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0f562-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="0f562-121">Il s’agit d’un élément enfant obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0f562-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="0f562-122">EndTime</span><span class="sxs-lookup"><span data-stu-id="0f562-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="0f562-123">Représente la fin d’un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0f562-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="0f562-124">Il s’agit d’un élément enfant obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0f562-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="0f562-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="0f562-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="0f562-126">Représente l’état de disponibilité défini pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0f562-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="0f562-127">Il s’agit d’un élément enfant obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0f562-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="0f562-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0f562-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="0f562-129">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0f562-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="0f562-130">Il s’agit d’un élément enfant facultatif.</span><span class="sxs-lookup"><span data-stu-id="0f562-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f562-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f562-131">Parent elements</span></span>

|<span data-ttu-id="0f562-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f562-132">**Element**</span></span>|<span data-ttu-id="0f562-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f562-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f562-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="0f562-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="0f562-135">Contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="0f562-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="0f562-136">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="0f562-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f562-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f562-137">Remarks</span></span>

<span data-ttu-id="0f562-138">Les heures de rendez-vous et de réunion sont renvoyées dans le fuseau horaire du client.</span><span class="sxs-lookup"><span data-stu-id="0f562-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="0f562-139">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent.</span><span class="sxs-lookup"><span data-stu-id="0f562-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="0f562-140">Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="0f562-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="0f562-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0f562-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f562-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f562-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f562-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f562-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f562-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f562-144">Schema Name</span></span>  <br/> |<span data-ttu-id="0f562-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0f562-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f562-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f562-146">Validation File</span></span>  <br/> |<span data-ttu-id="0f562-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f562-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f562-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f562-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f562-149">False</span><span class="sxs-lookup"><span data-stu-id="0f562-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f562-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f562-150">See also</span></span>



[<span data-ttu-id="0f562-151">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0f562-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0f562-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0f562-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0f562-153">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0f562-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

