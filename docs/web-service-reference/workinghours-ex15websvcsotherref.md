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
description: L’élément WorkingHours représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.
ms.openlocfilehash: 9cb21e72f7024b96b4b5f252a8a3b85bb704e67c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468340"
---
# <a name="workinghours"></a><span data-ttu-id="ae8bf-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="ae8bf-103">WorkingHours</span></span>

<span data-ttu-id="ae8bf-104">L’élément **WorkingHours** représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="ae8bf-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ae8bf-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ae8bf-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ae8bf-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ae8bf-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ae8bf-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ae8bf-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ae8bf-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ae8bf-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="ae8bf-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="ae8bf-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="ae8bf-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae8bf-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ae8bf-111">Attributes and elements</span></span>

<span data-ttu-id="ae8bf-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae8bf-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="ae8bf-113">Attributes</span></span>

<span data-ttu-id="ae8bf-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae8bf-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ae8bf-115">Child elements</span></span>

|<span data-ttu-id="ae8bf-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae8bf-116">**Element**</span></span>|<span data-ttu-id="ae8bf-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae8bf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae8bf-118">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="ae8bf-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="ae8bf-119">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="ae8bf-120">Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="ae8bf-121">Cet élément est requis si l’élément **WorkingHours** est utilisé.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="ae8bf-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="ae8bf-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="ae8bf-123">Contient des informations de période de travail pour l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="ae8bf-124">Cet élément est requis si l’élément **WorkingHours** est utilisé.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae8bf-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ae8bf-125">Parent elements</span></span>

|<span data-ttu-id="ae8bf-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae8bf-126">**Element**</span></span>|<span data-ttu-id="ae8bf-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae8bf-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae8bf-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ae8bf-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="ae8bf-129">Contient les informations de disponibilité d’un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="ae8bf-130">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ae8bf-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae8bf-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae8bf-131">Remarks</span></span>

<span data-ttu-id="ae8bf-132">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="ae8bf-133">Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="ae8bf-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ae8bf-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae8bf-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ae8bf-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae8bf-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ae8bf-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae8bf-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ae8bf-137">Schema Name</span></span>  <br/> |<span data-ttu-id="ae8bf-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ae8bf-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae8bf-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ae8bf-139">Validation File</span></span>  <br/> |<span data-ttu-id="ae8bf-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae8bf-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae8bf-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ae8bf-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae8bf-142">False</span><span class="sxs-lookup"><span data-stu-id="ae8bf-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae8bf-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae8bf-143">See also</span></span>



[<span data-ttu-id="ae8bf-144">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ae8bf-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ae8bf-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ae8bf-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ae8bf-146">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="ae8bf-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

