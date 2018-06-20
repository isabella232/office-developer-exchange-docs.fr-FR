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
ms.openlocfilehash: f7fff7ba511ca12813dd4c2d694e89c97589ba31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755463"
---
# <a name="calendarevent"></a><span data-ttu-id="ecb5b-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="ecb5b-103">CalendarEvent</span></span>

<span data-ttu-id="ecb5b-104">L’élément **CalendarEvent** représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="ecb5b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ecb5b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ecb5b-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ecb5b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ecb5b-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ecb5b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ecb5b-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ecb5b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ecb5b-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="ecb5b-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="ecb5b-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="ecb5b-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="ecb5b-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="ecb5b-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecb5b-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ecb5b-112">Attributes and elements</span></span>

<span data-ttu-id="ecb5b-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecb5b-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="ecb5b-114">Attributes</span></span>

<span data-ttu-id="ecb5b-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecb5b-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ecb5b-116">Child elements</span></span>

|<span data-ttu-id="ecb5b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ecb5b-117">**Element**</span></span>|<span data-ttu-id="ecb5b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ecb5b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecb5b-119">Heure de début</span><span class="sxs-lookup"><span data-stu-id="ecb5b-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="ecb5b-120">Représente le début d’un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="ecb5b-121">Il s’agit d’un élément enfant requis.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="ecb5b-122">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="ecb5b-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="ecb5b-123">Représente la fin d’un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="ecb5b-124">Il s’agit d’un élément enfant requis.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="ecb5b-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="ecb5b-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="ecb5b-126">Représente l’état de disponibilité pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="ecb5b-127">Il s’agit d’un élément enfant requis.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="ecb5b-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="ecb5b-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="ecb5b-129">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="ecb5b-130">Il s’agit d’un élément enfant facultatif.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ecb5b-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ecb5b-131">Parent elements</span></span>

|<span data-ttu-id="ecb5b-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ecb5b-132">**Element**</span></span>|<span data-ttu-id="ecb5b-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="ecb5b-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecb5b-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="ecb5b-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="ecb5b-135">Contient un ensemble d’occurrences d’élément calendrier unique représentant la disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="ecb5b-136">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ecb5b-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ecb5b-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="ecb5b-137">Remarks</span></span>

<span data-ttu-id="ecb5b-138">Les heures de rendez-vous et de réunion sont retournés dans le fuseau horaire du client.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="ecb5b-139">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="ecb5b-140">Le niveau de détail fourni par cet élément varie selon les autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="ecb5b-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ecb5b-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecb5b-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ecb5b-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecb5b-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ecb5b-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ecb5b-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ecb5b-144">Schema Name</span></span>  <br/> |<span data-ttu-id="ecb5b-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ecb5b-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="ecb5b-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ecb5b-146">Validation File</span></span>  <br/> |<span data-ttu-id="ecb5b-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ecb5b-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ecb5b-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ecb5b-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecb5b-149">False</span><span class="sxs-lookup"><span data-stu-id="ecb5b-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecb5b-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ecb5b-150">See also</span></span>



[<span data-ttu-id="ecb5b-151">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ecb5b-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ecb5b-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ecb5b-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ecb5b-153">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="ecb5b-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

