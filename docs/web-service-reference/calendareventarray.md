---
title: CalendarEventArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventArray
api_type:
- schema
ms.assetid: a00f7f56-d7f1-429d-ae02-97043718c864
description: L’élément CalendarEventArray contient un ensemble d’occurrences d’élément calendrier unique représentant la disponibilité de l’utilisateur demandé.
ms.openlocfilehash: 2e56b7b2b94e12401ba708dfca94101064d625e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755464"
---
# <a name="calendareventarray"></a><span data-ttu-id="1c537-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1c537-103">CalendarEventArray</span></span>

<span data-ttu-id="1c537-104">L’élément **CalendarEventArray** contient un ensemble d’occurrences d’élément calendrier unique représentant la disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="1c537-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="1c537-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1c537-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1c537-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1c537-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1c537-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1c537-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1c537-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1c537-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1c537-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1c537-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="1c537-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="1c537-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c537-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1c537-111">Attributes and elements</span></span>

<span data-ttu-id="1c537-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1c537-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c537-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="1c537-113">Attributes</span></span>

<span data-ttu-id="1c537-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c537-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c537-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1c537-115">Child elements</span></span>

|<span data-ttu-id="1c537-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c537-116">**Element**</span></span>|<span data-ttu-id="1c537-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c537-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c537-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1c537-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="1c537-119">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="1c537-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c537-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1c537-120">Parent elements</span></span>

|<span data-ttu-id="1c537-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c537-121">**Element**</span></span>|<span data-ttu-id="1c537-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c537-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c537-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1c537-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="1c537-124">Contient des informations de disponibilité pour un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="1c537-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="1c537-125">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1c537-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c537-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="1c537-126">Remarks</span></span>

<span data-ttu-id="1c537-127">Le niveau de détail fourni par cet élément varie selon les autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="1c537-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="1c537-128">Cet élément est inclus lors de l’élément [FreeBusyViewType](freebusyviewtype.md) est défini sur **FreeBusy**, **FreeBusyMerged**, **détaillé**ou **DetailedMerged**.</span><span class="sxs-lookup"><span data-stu-id="1c537-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="1c537-129">Cet élément n’inclut pas tous les éléments enfants si aucun élément de calendrier n’est présents dans la fenêtre de temps demandé.</span><span class="sxs-lookup"><span data-stu-id="1c537-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="1c537-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1c537-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c537-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1c537-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c537-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1c537-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c537-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1c537-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1c537-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1c537-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c537-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1c537-135">Validation File</span></span>  <br/> |<span data-ttu-id="1c537-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c537-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c537-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1c537-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c537-138">False</span><span class="sxs-lookup"><span data-stu-id="1c537-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c537-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1c537-139">See also</span></span>



[<span data-ttu-id="1c537-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1c537-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1c537-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1c537-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1c537-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1c537-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

