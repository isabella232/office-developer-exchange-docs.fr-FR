---
title: IsRecurring (CalendarEventDetails)
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
ms.assetid: 42323940-0ccb-4a05-86e4-262bde5e41b0
description: L’élément IsRecurring indique si l’événement du calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.
ms.openlocfilehash: 87a168dc48bdd5ba2ea9398dd84f696e7729db44
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828103"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="47a69-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="47a69-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="47a69-104">L’élément **IsRecurring** indique si l’événement du calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="47a69-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="47a69-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="47a69-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="47a69-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="47a69-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="47a69-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="47a69-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="47a69-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="47a69-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="47a69-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="47a69-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="47a69-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="47a69-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="47a69-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="47a69-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="47a69-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="47a69-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="47a69-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="47a69-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47a69-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="47a69-114">Attributes and elements</span></span>

<span data-ttu-id="47a69-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="47a69-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47a69-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="47a69-116">Attributes</span></span>

<span data-ttu-id="47a69-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="47a69-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47a69-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="47a69-118">Child elements</span></span>

<span data-ttu-id="47a69-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="47a69-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47a69-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="47a69-120">Parent elements</span></span>

|<span data-ttu-id="47a69-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="47a69-121">**Element**</span></span>|<span data-ttu-id="47a69-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="47a69-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47a69-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="47a69-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="47a69-124">Fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="47a69-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="47a69-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="47a69-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47a69-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="47a69-126">Text value</span></span>

<span data-ttu-id="47a69-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="47a69-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="47a69-128">Cet élément est obligatoire si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="47a69-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="47a69-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="47a69-129">Remarks</span></span>

<span data-ttu-id="47a69-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="47a69-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47a69-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="47a69-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47a69-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="47a69-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47a69-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="47a69-133">Schema Name</span></span>  <br/> |<span data-ttu-id="47a69-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="47a69-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="47a69-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="47a69-135">Validation File</span></span>  <br/> |<span data-ttu-id="47a69-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47a69-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47a69-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="47a69-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="47a69-138">False</span><span class="sxs-lookup"><span data-stu-id="47a69-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47a69-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="47a69-139">See also</span></span>



[<span data-ttu-id="47a69-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="47a69-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="47a69-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="47a69-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="47a69-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="47a69-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

