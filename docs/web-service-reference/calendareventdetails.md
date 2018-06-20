---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: L’élément CalendarEventDetails fournit des informations supplémentaires sur un événement de calendrier.
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755465"
---
# <a name="calendareventdetails"></a><span data-ttu-id="da1f3-103">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="da1f3-103">CalendarEventDetails</span></span>

<span data-ttu-id="da1f3-104">L’élément **CalendarEventDetails** fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="da1f3-104">The **CalendarEventDetails** element provides additional information about a calendar event.</span></span> 
  
[<span data-ttu-id="da1f3-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="da1f3-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="da1f3-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="da1f3-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="da1f3-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="da1f3-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="da1f3-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="da1f3-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="da1f3-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="da1f3-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="da1f3-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="da1f3-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="da1f3-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="da1f3-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 <span data-ttu-id="da1f3-112">**CalendarEventDetails**</span><span class="sxs-lookup"><span data-stu-id="da1f3-112">**CalendarEventDetails**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da1f3-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="da1f3-113">Attributes and elements</span></span>

<span data-ttu-id="da1f3-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="da1f3-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da1f3-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="da1f3-115">Attributes</span></span>

<span data-ttu-id="da1f3-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="da1f3-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da1f3-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="da1f3-117">Child elements</span></span>

|<span data-ttu-id="da1f3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="da1f3-118">**Element**</span></span>|<span data-ttu-id="da1f3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="da1f3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da1f3-120">ID</span><span class="sxs-lookup"><span data-stu-id="da1f3-120">ID</span></span>](id.md) <br/> |<span data-ttu-id="da1f3-121">Représente l’identificateur d’entrée de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="da1f3-121">Represents the entry ID of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-122">Sujet (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="da1f3-122">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md) <br/> |<span data-ttu-id="da1f3-123">Représente l’objet de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="da1f3-123">Represents the subject of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-124">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="da1f3-124">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md) <br/> |<span data-ttu-id="da1f3-125">Représente le champ emplacement de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="da1f3-125">Represents the location field of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-126">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="da1f3-126">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md) <br/> |<span data-ttu-id="da1f3-127">Indique si l’événement du calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="da1f3-127">Indicates whether the calendar event is a meeting or an appointment.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-128">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="da1f3-128">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md) <br/> |<span data-ttu-id="da1f3-129">Indique si l’événement du calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="da1f3-129">Indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-130">IsException</span><span class="sxs-lookup"><span data-stu-id="da1f3-130">IsException</span></span>](isexception.md) <br/> |<span data-ttu-id="da1f3-131">Indique si une instance d’un élément de calendrier périodique est modifiée à partir de la forme de base.</span><span class="sxs-lookup"><span data-stu-id="da1f3-131">Indicates whether an instance of a recurring calendar item is changed from the master.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-132">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="da1f3-132">IsReminderSet</span></span>](isreminderset.md) <br/> |<span data-ttu-id="da1f3-133">Indique si un rappel a été défini pour l’événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="da1f3-133">Indicates whether a reminder has been set for the calendar event.</span></span>  <br/> |
|[<span data-ttu-id="da1f3-134">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="da1f3-134">IsPrivate</span></span>](isprivate.md) <br/> |<span data-ttu-id="da1f3-135">Indique si l’élément de calendrier est privé.</span><span class="sxs-lookup"><span data-stu-id="da1f3-135">Indicates whether the calendar item is private.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da1f3-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="da1f3-136">Parent elements</span></span>

|<span data-ttu-id="da1f3-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="da1f3-137">**Element**</span></span>|<span data-ttu-id="da1f3-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="da1f3-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da1f3-139">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="da1f3-139">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="da1f3-140">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="da1f3-140">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="da1f3-141">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="da1f3-141">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da1f3-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="da1f3-142">Remarks</span></span>

<span data-ttu-id="da1f3-143">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent.</span><span class="sxs-lookup"><span data-stu-id="da1f3-143">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="da1f3-144">Si l’élément [IsPrivate](isprivate.md) a la **valeur true**, tous les autres éléments dans l’élément [CalendarEventDetails](calendareventdetails.md) ne sont pas renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="da1f3-144">If the [IsPrivate](isprivate.md) element is **true**, all the other elements in the [CalendarEventDetails](calendareventdetails.md) element are not returned in the response.</span></span> 
  
<span data-ttu-id="da1f3-145">L’opération GetUserAvailability ne renvoie pas d’informations détaillées sur l’appelant, sauf si l’appelant dispose d’un accès en lecture sur le calendrier de l’utilisateur cible.</span><span class="sxs-lookup"><span data-stu-id="da1f3-145">The GetUserAvailability operation does not return detailed caller information unless the caller has read access on the target user's calendar.</span></span> <span data-ttu-id="da1f3-146">Vous pouvez définir des autorisations d’accès à l’aide de l’environnement Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="da1f3-146">You can set access permissions by using the Exchange Management Shell.</span></span>
  
<span data-ttu-id="da1f3-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="da1f3-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da1f3-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="da1f3-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da1f3-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="da1f3-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da1f3-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="da1f3-150">Schema Name</span></span>  <br/> |<span data-ttu-id="da1f3-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="da1f3-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="da1f3-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="da1f3-152">Validation File</span></span>  <br/> |<span data-ttu-id="da1f3-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da1f3-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da1f3-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="da1f3-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="da1f3-155">False</span><span class="sxs-lookup"><span data-stu-id="da1f3-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da1f3-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="da1f3-156">See also</span></span>



[<span data-ttu-id="da1f3-157">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="da1f3-157">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="da1f3-158">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="da1f3-158">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="da1f3-159">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="da1f3-159">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

