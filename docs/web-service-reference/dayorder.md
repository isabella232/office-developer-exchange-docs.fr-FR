---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: L’élément DayOrder représente la nième occurrence du jour spécifié dans l’élément DayOfWeek (fuseau horaire) qui représente la date de transition d’et à l’heure standard et l’heure d’été.
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755824"
---
# <a name="dayorder"></a><span data-ttu-id="d185e-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="d185e-103">DayOrder</span></span>

<span data-ttu-id="d185e-104">L’élément **DayOrder** représente l’occurrence _n_th de la journée spécifiée dans l’élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui représente la date de transition d’et à l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="d185e-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="d185e-105">**court**</span><span class="sxs-lookup"><span data-stu-id="d185e-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d185e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d185e-106">Attributes and elements</span></span>

<span data-ttu-id="d185e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d185e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d185e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d185e-108">Attributes</span></span>

<span data-ttu-id="d185e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d185e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d185e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d185e-110">Child elements</span></span>

<span data-ttu-id="d185e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d185e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d185e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d185e-112">Parent elements</span></span>

|<span data-ttu-id="d185e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d185e-113">**Element**</span></span>|<span data-ttu-id="d185e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d185e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d185e-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="d185e-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="d185e-116">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="d185e-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="d185e-117">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="d185e-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="d185e-118">Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d185e-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="d185e-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="d185e-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="d185e-120">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="d185e-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="d185e-121">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="d185e-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="d185e-122">Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d185e-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d185e-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d185e-123">Text value</span></span>

<span data-ttu-id="d185e-124">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d185e-124">A text value is required.</span></span> <span data-ttu-id="d185e-125">La valeur de l’élément **DayOrder** peut être de 1 à 5.</span><span class="sxs-lookup"><span data-stu-id="d185e-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="d185e-126">La valeur maximale pour cet élément peut être 4 ou 5, selon le mois et l’année.</span><span class="sxs-lookup"><span data-stu-id="d185e-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d185e-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="d185e-127">Remarks</span></span>

<span data-ttu-id="d185e-128">Un élément [StandardTime](standardtime.md) qui contient un élément **DayOrder** qui a une valeur de 5, un élément [mois](month.md) qui a une valeur de 10 et un élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui a une valeur de dimanche signifie que la transition à partir de l’heure l’heure d’été se produit le dimanche cinquième du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="d185e-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d185e-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d185e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d185e-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d185e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d185e-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d185e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d185e-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d185e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d185e-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d185e-133">Validation File</span></span>  <br/> |<span data-ttu-id="d185e-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d185e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d185e-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d185e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d185e-136">False</span><span class="sxs-lookup"><span data-stu-id="d185e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d185e-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d185e-137">See also</span></span>

- [<span data-ttu-id="d185e-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d185e-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d185e-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d185e-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

