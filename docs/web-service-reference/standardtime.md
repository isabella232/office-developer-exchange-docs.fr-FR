---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: L’élément StandardTime représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément Bias (UTC). Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829546"
---
# <a name="standardtime"></a><span data-ttu-id="7c591-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="7c591-104">StandardTime</span></span>

<span data-ttu-id="7c591-105">L’élément **StandardTime** représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="7c591-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="7c591-106">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="7c591-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="7c591-107">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="7c591-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="7c591-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="7c591-108">StandardTime</span></span>](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 <span data-ttu-id="7c591-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="7c591-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c591-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7c591-110">Attributes and elements</span></span>

<span data-ttu-id="7c591-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7c591-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c591-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="7c591-112">Attributes</span></span>

<span data-ttu-id="7c591-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c591-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c591-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7c591-114">Child elements</span></span>

|<span data-ttu-id="7c591-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c591-115">**Element**</span></span>|<span data-ttu-id="7c591-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c591-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c591-117">Bias</span><span class="sxs-lookup"><span data-stu-id="7c591-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="7c591-118">Représente le décalage de l’offset UTC identifié par l’élément [Bias (UTC)](bias-utc.md) heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="7c591-119">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="7c591-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="7c591-120">Heure</span><span class="sxs-lookup"><span data-stu-id="7c591-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="7c591-121">Représente le temps de transition de la journée à et d’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7c591-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="7c591-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="7c591-123">Représente l’occurrence _n_th de la journée qui est spécifiée dans l’élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui représente la date de transition d’et à l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7c591-124">Mois</span><span class="sxs-lookup"><span data-stu-id="7c591-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="7c591-125">Représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7c591-126">DayOfWeek (fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="7c591-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="7c591-127">Représente le jour de la semaine quand se produit la transition vers et depuis l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="7c591-128">Année</span><span class="sxs-lookup"><span data-stu-id="7c591-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="7c591-129">Définit un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="7c591-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="7c591-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7c591-130">This element is optional.</span></span> <span data-ttu-id="7c591-131">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7c591-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c591-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7c591-132">Parent elements</span></span>

|<span data-ttu-id="7c591-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c591-133">**Element**</span></span>|<span data-ttu-id="7c591-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c591-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c591-135">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="7c591-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="7c591-136">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7c591-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="7c591-137">Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7c591-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="7c591-138">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7c591-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c591-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="7c591-139">Remarks</span></span>

<span data-ttu-id="7c591-140">L’élément **StandardTime** représente une heure de décalage est représentée par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="7c591-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="7c591-141">Lorsque l’élément [Bias](bias.md) enfant est égale à 0, le temps standard est égal à l’offset bias UTC est représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="7c591-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="7c591-142">Exemple</span><span class="sxs-lookup"><span data-stu-id="7c591-142">Example</span></span>

<span data-ttu-id="7c591-143">L’exemple suivant montre une zone où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="7c591-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="7c591-144">La transition à partir de l’heure d’été à l’heure standard est observée à 2 heures.</span><span class="sxs-lookup"><span data-stu-id="7c591-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="7c591-145">le cinquième dimanche du mois dixième.</span><span class="sxs-lookup"><span data-stu-id="7c591-145">on the fifth Sunday of the tenth month.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="7c591-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7c591-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c591-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7c591-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c591-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7c591-148">Schema Name</span></span>  <br/> |<span data-ttu-id="7c591-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7c591-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c591-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7c591-150">Validation File</span></span>  <br/> |<span data-ttu-id="7c591-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c591-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c591-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7c591-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c591-153">False</span><span class="sxs-lookup"><span data-stu-id="7c591-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c591-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7c591-154">See also</span></span>

- [<span data-ttu-id="7c591-155">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7c591-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7c591-156">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="7c591-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

