---
title: Heure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: L’élément heure représente le temps de transition de la journée à et d’heure standard et l’heure d’été.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838700"
---
# <a name="time"></a><span data-ttu-id="555a6-103">Heure</span><span class="sxs-lookup"><span data-stu-id="555a6-103">Time</span></span>

<span data-ttu-id="555a6-104">L’élément **heure** représente le temps de transition de la journée à et d’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="555a6-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="555a6-105">**string**</span><span class="sxs-lookup"><span data-stu-id="555a6-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="555a6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="555a6-106">Attributes and elements</span></span>

<span data-ttu-id="555a6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="555a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="555a6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="555a6-108">Attributes</span></span>

<span data-ttu-id="555a6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="555a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="555a6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="555a6-110">Child elements</span></span>

<span data-ttu-id="555a6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="555a6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="555a6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="555a6-112">Parent elements</span></span>

|<span data-ttu-id="555a6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="555a6-113">**Element**</span></span>|<span data-ttu-id="555a6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="555a6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="555a6-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="555a6-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="555a6-116">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="555a6-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="555a6-117">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="555a6-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="555a6-118">Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="555a6-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="555a6-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="555a6-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="555a6-120">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="555a6-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="555a6-121">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="555a6-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="555a6-122">Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="555a6-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="555a6-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="555a6-123">Text value</span></span>

<span data-ttu-id="555a6-124">La valeur de texte représente les heures, minutes et secondes sous la forme suivante : hh : mm :.</span><span class="sxs-lookup"><span data-stu-id="555a6-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="555a6-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="555a6-125">Remarks</span></span>

<span data-ttu-id="555a6-126">En cas de l’élément de **temps** dans l’élément [DaylightTime](daylighttime.md) , il représente l’heure du jour qui se produit la transition à partir de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="555a6-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="555a6-127">En cas de l’élément de [temps](time.md) dans l’élément [StandardTime](standardtime.md) , il représente l’heure du jour qui se produit la transition à partir de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="555a6-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="555a6-128">Cet élément a une occurrence minimale de zéro et une occurrence d’un maximum.</span><span class="sxs-lookup"><span data-stu-id="555a6-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="555a6-129">Exemple</span><span class="sxs-lookup"><span data-stu-id="555a6-129">Example</span></span>

<span data-ttu-id="555a6-130">La partie suivante d’une demande représente un temps de transition de 2 heures.</span><span class="sxs-lookup"><span data-stu-id="555a6-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="555a6-131">à partir de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="555a6-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="555a6-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="555a6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="555a6-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="555a6-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="555a6-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="555a6-134">Schema Name</span></span>  <br/> |<span data-ttu-id="555a6-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="555a6-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="555a6-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="555a6-136">Validation File</span></span>  <br/> |<span data-ttu-id="555a6-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="555a6-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="555a6-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="555a6-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="555a6-139">False</span><span class="sxs-lookup"><span data-stu-id="555a6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="555a6-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="555a6-140">See also</span></span>

- [<span data-ttu-id="555a6-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="555a6-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="555a6-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="555a6-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

