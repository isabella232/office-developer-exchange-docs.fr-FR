---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: L’élément Bias représente le décalage de l’offset de temps universel coordonné (UTC) identifié par l’élément Bias (UTC) heure standard et l’heure d’été. Cette valeur est exprimée en minutes.
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755389"
---
# <a name="bias"></a><span data-ttu-id="f7bbb-104">Bias</span><span class="sxs-lookup"><span data-stu-id="f7bbb-104">Bias</span></span>

<span data-ttu-id="f7bbb-105">L’élément **Bias** représente le décalage de l’offset de temps universel coordonné (UTC) identifié par l’élément [Bias (UTC)](bias-utc.md) heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="f7bbb-106">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="f7bbb-107">**int**</span><span class="sxs-lookup"><span data-stu-id="f7bbb-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f7bbb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7bbb-108">Attributes and elements</span></span>

<span data-ttu-id="f7bbb-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7bbb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7bbb-110">Attributes</span></span>

<span data-ttu-id="f7bbb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7bbb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7bbb-112">Child elements</span></span>

<span data-ttu-id="f7bbb-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7bbb-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7bbb-114">Parent elements</span></span>

|<span data-ttu-id="f7bbb-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7bbb-115">**Element**</span></span>|<span data-ttu-id="f7bbb-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7bbb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7bbb-117">StandardTime</span><span class="sxs-lookup"><span data-stu-id="f7bbb-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="f7bbb-118">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f7bbb-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="f7bbb-119">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="f7bbb-120">Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="f7bbb-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="f7bbb-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="f7bbb-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="f7bbb-122">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="f7bbb-123">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="f7bbb-124">Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="f7bbb-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7bbb-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f7bbb-125">Text value</span></span>

<span data-ttu-id="f7bbb-126">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-126">A text value is required.</span></span> <span data-ttu-id="f7bbb-127">La valeur de texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7bbb-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7bbb-128">Remarks</span></span>

<span data-ttu-id="f7bbb-129">Le décalage permet de déterminer l’heure locale seulement peut être assurée par un des éléments de **l’écart** .</span><span class="sxs-lookup"><span data-stu-id="f7bbb-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="f7bbb-130">La somme des valeurs de l’élément Bias fournies par l’élément [DaylightTime](daylighttime.md) ou l’élément [StandardTime](standardtime.md) ainsi que l’élément [Bias (UTC)](bias-utc.md) identifie l’heure locale.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="f7bbb-131">Exemple</span><span class="sxs-lookup"><span data-stu-id="f7bbb-131">Example</span></span>

<span data-ttu-id="f7bbb-132">L’exemple suivant montre une partie d’une requête XML qui identifie un utilisateur qui observe l’heure d’été en ajustant le décalage de l’heure UTC à 60 minutes.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="f7bbb-133">Cela rend l’écart 420 minutes à l’heure UTC.</span><span class="sxs-lookup"><span data-stu-id="f7bbb-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="f7bbb-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7bbb-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7bbb-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7bbb-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7bbb-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7bbb-136">Schema Name</span></span>  <br/> |<span data-ttu-id="f7bbb-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f7bbb-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7bbb-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7bbb-138">Validation File</span></span>  <br/> |<span data-ttu-id="f7bbb-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7bbb-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7bbb-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7bbb-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7bbb-141">False</span><span class="sxs-lookup"><span data-stu-id="f7bbb-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7bbb-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7bbb-142">See also</span></span>

- [<span data-ttu-id="f7bbb-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f7bbb-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="f7bbb-144">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="f7bbb-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

