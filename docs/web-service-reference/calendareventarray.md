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
description: L’élément CalendarEventArray contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.
ms.openlocfilehash: 6badba2477a9d48c6d109740de454e2815d3c211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463369"
---
# <a name="calendareventarray"></a><span data-ttu-id="e5292-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="e5292-103">CalendarEventArray</span></span>

<span data-ttu-id="e5292-104">L’élément **CalendarEventArray** contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="e5292-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="e5292-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5292-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e5292-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="e5292-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="e5292-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="e5292-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="e5292-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e5292-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="e5292-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="e5292-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="e5292-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="e5292-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5292-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e5292-111">Attributes and elements</span></span>

<span data-ttu-id="e5292-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e5292-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5292-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="e5292-113">Attributes</span></span>

<span data-ttu-id="e5292-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e5292-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5292-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e5292-115">Child elements</span></span>

|<span data-ttu-id="e5292-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e5292-116">**Element**</span></span>|<span data-ttu-id="e5292-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e5292-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5292-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="e5292-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="e5292-119">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="e5292-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5292-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e5292-120">Parent elements</span></span>

|<span data-ttu-id="e5292-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e5292-121">**Element**</span></span>|<span data-ttu-id="e5292-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="e5292-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5292-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e5292-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="e5292-124">Contient les informations de disponibilité d’un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="e5292-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="e5292-125">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e5292-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e5292-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="e5292-126">Remarks</span></span>

<span data-ttu-id="e5292-127">Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="e5292-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="e5292-128">Cet élément est inclus lorsque l’élément [FreeBusyViewType](freebusyviewtype.md) est défini sur **freebusy**, **FreeBusyMerged**, **detailed**ou **DetailedMerged**.</span><span class="sxs-lookup"><span data-stu-id="e5292-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="e5292-129">Cet élément n’inclut aucun élément enfant si aucun élément de calendrier n’est présent dans la fenêtre de temps demandée.</span><span class="sxs-lookup"><span data-stu-id="e5292-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="e5292-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e5292-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5292-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e5292-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5292-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e5292-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5292-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e5292-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e5292-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e5292-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5292-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e5292-135">Validation File</span></span>  <br/> |<span data-ttu-id="e5292-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5292-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5292-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e5292-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5292-138">False</span><span class="sxs-lookup"><span data-stu-id="e5292-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5292-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e5292-139">See also</span></span>



[<span data-ttu-id="e5292-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e5292-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e5292-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5292-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e5292-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e5292-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

