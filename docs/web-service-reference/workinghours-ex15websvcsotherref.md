---
title: WorkingHours
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: L’élément WorkingHours représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.
ms.openlocfilehash: c53779422b87adebed370a1ed88e4e91c7a2dcaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839056"
---
# <a name="workinghours"></a><span data-ttu-id="b78d4-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="b78d4-103">WorkingHours</span></span>

<span data-ttu-id="b78d4-104">L’élément **WorkingHours** représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.</span><span class="sxs-lookup"><span data-stu-id="b78d4-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="b78d4-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b78d4-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b78d4-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b78d4-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b78d4-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b78d4-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b78d4-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b78d4-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b78d4-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="b78d4-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="b78d4-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="b78d4-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b78d4-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b78d4-111">Attributes and elements</span></span>

<span data-ttu-id="b78d4-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b78d4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b78d4-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="b78d4-113">Attributes</span></span>

<span data-ttu-id="b78d4-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b78d4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b78d4-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b78d4-115">Child elements</span></span>

|<span data-ttu-id="b78d4-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b78d4-116">**Element**</span></span>|<span data-ttu-id="b78d4-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b78d4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b78d4-118">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="b78d4-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="b78d4-119">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="b78d4-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="b78d4-120">Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="b78d4-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="b78d4-121">Cet élément est obligatoire si l’élément **WorkingHours** est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b78d4-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="b78d4-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="b78d4-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="b78d4-123">Contient des informations sur les périodes de l’utilisateur de boîte aux lettres de travail.</span><span class="sxs-lookup"><span data-stu-id="b78d4-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="b78d4-124">Cet élément est obligatoire si l’élément **WorkingHours** est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b78d4-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b78d4-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b78d4-125">Parent elements</span></span>

|<span data-ttu-id="b78d4-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b78d4-126">**Element**</span></span>|<span data-ttu-id="b78d4-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="b78d4-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b78d4-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b78d4-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="b78d4-129">Contient des informations de disponibilité pour un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="b78d4-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="b78d4-130">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b78d4-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b78d4-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="b78d4-131">Remarks</span></span>

<span data-ttu-id="b78d4-132">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent.</span><span class="sxs-lookup"><span data-stu-id="b78d4-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="b78d4-133">Le niveau de détail fourni par cet élément varie selon les autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="b78d4-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="b78d4-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b78d4-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b78d4-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b78d4-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b78d4-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b78d4-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b78d4-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b78d4-137">Schema Name</span></span>  <br/> |<span data-ttu-id="b78d4-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b78d4-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="b78d4-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b78d4-139">Validation File</span></span>  <br/> |<span data-ttu-id="b78d4-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b78d4-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b78d4-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b78d4-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="b78d4-142">False</span><span class="sxs-lookup"><span data-stu-id="b78d4-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b78d4-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b78d4-143">See also</span></span>



[<span data-ttu-id="b78d4-144">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b78d4-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b78d4-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b78d4-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b78d4-146">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="b78d4-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

