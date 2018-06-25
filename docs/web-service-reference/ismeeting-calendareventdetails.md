---
title: IsMeeting (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: L’élément IsMeeting indique si l’événement du calendrier est une réunion ou un rendez-vous.
ms.openlocfilehash: f3f6e0cc5fbfe29e5a818d69794cbaf5b6855962
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828046"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="1c1d7-103">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1c1d7-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="1c1d7-104">L’élément **IsMeeting** indique si l’événement du calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="1c1d7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1c1d7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1c1d7-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1c1d7-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1c1d7-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1c1d7-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1c1d7-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1c1d7-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1c1d7-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1c1d7-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="1c1d7-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1c1d7-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="1c1d7-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1c1d7-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="1c1d7-112">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1c1d7-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="1c1d7-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="1c1d7-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c1d7-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1c1d7-114">Attributes and elements</span></span>

<span data-ttu-id="1c1d7-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c1d7-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="1c1d7-116">Attributes</span></span>

<span data-ttu-id="1c1d7-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c1d7-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1c1d7-118">Child elements</span></span>

<span data-ttu-id="1c1d7-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c1d7-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1c1d7-120">Parent elements</span></span>

|<span data-ttu-id="1c1d7-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c1d7-121">**Element**</span></span>|<span data-ttu-id="1c1d7-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c1d7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c1d7-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1c1d7-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="1c1d7-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="1c1d7-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c1d7-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c1d7-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1c1d7-126">Text value</span></span>

<span data-ttu-id="1c1d7-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="1c1d7-128">Cet élément est obligatoire si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1c1d7-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="1c1d7-129">Remarks</span></span>

<span data-ttu-id="1c1d7-130">La différence entre une réunion et un rendez-vous est une réunion un élément de calendrier qui inclut des participants ; un rendez-vous est un élément de calendrier qui n’inclut pas les participants.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="1c1d7-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c1d7-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1c1d7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c1d7-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1c1d7-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c1d7-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1c1d7-134">Schema Name</span></span>  <br/> |<span data-ttu-id="1c1d7-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1c1d7-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c1d7-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1c1d7-136">Validation File</span></span>  <br/> |<span data-ttu-id="1c1d7-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c1d7-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c1d7-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1c1d7-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c1d7-139">False</span><span class="sxs-lookup"><span data-stu-id="1c1d7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c1d7-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1c1d7-140">See also</span></span>



[<span data-ttu-id="1c1d7-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1c1d7-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1c1d7-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1c1d7-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1c1d7-143">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1c1d7-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

