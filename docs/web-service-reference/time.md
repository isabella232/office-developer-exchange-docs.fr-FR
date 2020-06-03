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
description: L’élément Time représente le temps de transition entre le jour et l’heure standard et l’heure d’été.
ms.openlocfilehash: 97c89fbcbdb85fcdd4d32a1d44075ac42adef053
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460294"
---
# <a name="time"></a><span data-ttu-id="c31e9-103">Time</span><span class="sxs-lookup"><span data-stu-id="c31e9-103">Time</span></span>

<span data-ttu-id="c31e9-104">L’élément **Time** représente le temps de transition entre le jour et l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c31e9-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="c31e9-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="c31e9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c31e9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c31e9-106">Attributes and elements</span></span>

<span data-ttu-id="c31e9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c31e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c31e9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c31e9-108">Attributes</span></span>

<span data-ttu-id="c31e9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c31e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c31e9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c31e9-110">Child elements</span></span>

<span data-ttu-id="c31e9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c31e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c31e9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c31e9-112">Parent elements</span></span>

|<span data-ttu-id="c31e9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c31e9-113">**Element**</span></span>|<span data-ttu-id="c31e9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c31e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c31e9-115">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="c31e9-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="c31e9-116">Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="c31e9-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="c31e9-117">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="c31e9-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="c31e9-118">Voici les expressions XPath de l’élément [StandardTime Element](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="c31e9-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="c31e9-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="c31e9-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="c31e9-120">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="c31e9-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="c31e9-121">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="c31e9-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="c31e9-122">Voici les expressions XPath de l’élément [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="c31e9-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c31e9-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c31e9-123">Text value</span></span>

<span data-ttu-id="c31e9-124">La valeur texte représente les heures, les minutes et les secondes dans le format suivant : HH : mm : SS.</span><span class="sxs-lookup"><span data-stu-id="c31e9-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c31e9-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="c31e9-125">Remarks</span></span>

<span data-ttu-id="c31e9-126">Lorsque l’élément **Time** se produit dans l’élément [DaylightTime](daylighttime.md) , il représente l’heure du jour où se produit la transition entre l’heure d’été et l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="c31e9-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="c31e9-127">Lorsque l’élément [Time](time.md) se produit dans l’élément [StandardTime Element](standardtime.md) , il représente l’heure du jour où se produit la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c31e9-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="c31e9-128">Cet élément a une occurrence minimale de zéro et une occurrence maximale d’un.</span><span class="sxs-lookup"><span data-stu-id="c31e9-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="c31e9-129">Exemple</span><span class="sxs-lookup"><span data-stu-id="c31e9-129">Example</span></span>

<span data-ttu-id="c31e9-130">La partie suivante d’une requête représente le temps de transition de 2 heures.</span><span class="sxs-lookup"><span data-stu-id="c31e9-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="c31e9-131">de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c31e9-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="c31e9-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c31e9-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c31e9-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c31e9-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c31e9-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c31e9-134">Schema Name</span></span>  <br/> |<span data-ttu-id="c31e9-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c31e9-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="c31e9-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c31e9-136">Validation File</span></span>  <br/> |<span data-ttu-id="c31e9-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c31e9-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c31e9-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c31e9-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="c31e9-139">False</span><span class="sxs-lookup"><span data-stu-id="c31e9-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c31e9-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c31e9-140">See also</span></span>

- [<span data-ttu-id="c31e9-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c31e9-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c31e9-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c31e9-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

