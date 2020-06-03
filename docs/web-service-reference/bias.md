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
description: L’élément Bias représente le décalage par rapport à l’offset UTC (temps universel coordonné) identifié par l’élément bias (UTC) pour l’heure standard et l’heure d’été. Cette valeur est exprimée en minutes.
ms.openlocfilehash: 6c9dce88f3eece9c793fb018114f07a85c7cb89b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460238"
---
# <a name="bias"></a><span data-ttu-id="9a080-104">Bias</span><span class="sxs-lookup"><span data-stu-id="9a080-104">Bias</span></span>

<span data-ttu-id="9a080-105">L’élément **Bias** représente le décalage par rapport à l’offset UTC (temps universel coordonné) identifié par l’élément [bias (UTC)](bias-utc.md) pour l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9a080-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="9a080-106">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="9a080-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="9a080-107">**int**</span><span class="sxs-lookup"><span data-stu-id="9a080-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9a080-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a080-108">Attributes and elements</span></span>

<span data-ttu-id="9a080-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a080-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a080-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a080-110">Attributes</span></span>

<span data-ttu-id="9a080-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9a080-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a080-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a080-112">Child elements</span></span>

<span data-ttu-id="9a080-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a080-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a080-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a080-114">Parent elements</span></span>

|<span data-ttu-id="9a080-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a080-115">**Element**</span></span>|<span data-ttu-id="9a080-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a080-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a080-117">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="9a080-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="9a080-118">Représente un décalage par rapport à l’heure par rapport à l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="9a080-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="9a080-119">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="9a080-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="9a080-120">Voici les expressions XPath de l’élément [StandardTime Element](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="9a080-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="9a080-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="9a080-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="9a080-122">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="9a080-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="9a080-123">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="9a080-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="9a080-124">Voici les expressions XPath de l’élément [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="9a080-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a080-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9a080-125">Text value</span></span>

<span data-ttu-id="9a080-126">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="9a080-126">A text value is required.</span></span> <span data-ttu-id="9a080-127">La valeur texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="9a080-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a080-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a080-128">Remarks</span></span>

<span data-ttu-id="9a080-129">L’offset utilisé pour déterminer l’heure locale ne peut être fourni que par l’un des éléments **Bias** .</span><span class="sxs-lookup"><span data-stu-id="9a080-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="9a080-130">La somme des valeurs de l’élément Bias fourni par l’élément [DaylightTime](daylighttime.md) ou l’élément [StandardTime Element](standardtime.md) plus l’élément [bias (UTC)](bias-utc.md) identifie l’heure locale.</span><span class="sxs-lookup"><span data-stu-id="9a080-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="9a080-131">Exemple</span><span class="sxs-lookup"><span data-stu-id="9a080-131">Example</span></span>

<span data-ttu-id="9a080-132">L’exemple suivant montre une partie d’une requête XML qui identifie un utilisateur qui observe l’heure d’été en ajustant le décalage par rapport à l’heure UTC par-60 minutes.</span><span class="sxs-lookup"><span data-stu-id="9a080-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="9a080-133">Cela fait le décalage de 420 minutes par rapport à l’heure UTC.</span><span class="sxs-lookup"><span data-stu-id="9a080-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="9a080-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a080-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a080-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a080-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a080-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a080-136">Schema Name</span></span>  <br/> |<span data-ttu-id="9a080-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9a080-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a080-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a080-138">Validation File</span></span>  <br/> |<span data-ttu-id="9a080-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9a080-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a080-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a080-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a080-141">False</span><span class="sxs-lookup"><span data-stu-id="9a080-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a080-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a080-142">See also</span></span>

- [<span data-ttu-id="9a080-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9a080-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="9a080-144">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9a080-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

