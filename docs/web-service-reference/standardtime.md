---
title: StandardTime Element
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
description: L’élément StandardTime Element représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément bias (UTC). Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456401"
---
# <a name="standardtime"></a><span data-ttu-id="c6823-104">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="c6823-104">StandardTime</span></span>

<span data-ttu-id="c6823-105">L’élément **StandardTime Element** représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="c6823-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="c6823-106">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="c6823-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="c6823-107">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="c6823-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="c6823-108">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="c6823-108">StandardTime</span></span>](standardtime.md)
  
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

 <span data-ttu-id="c6823-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="c6823-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6823-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6823-110">Attributes and elements</span></span>

<span data-ttu-id="c6823-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6823-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6823-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6823-112">Attributes</span></span>

<span data-ttu-id="c6823-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c6823-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6823-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6823-114">Child elements</span></span>

|<span data-ttu-id="c6823-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6823-115">**Element**</span></span>|<span data-ttu-id="c6823-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6823-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6823-117">Bias</span><span class="sxs-lookup"><span data-stu-id="c6823-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="c6823-118">Représente le décalage à partir de l’offset UTC identifié par l’élément [bias (UTC)](bias-utc.md) pour l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="c6823-119">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="c6823-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="c6823-120">Time</span><span class="sxs-lookup"><span data-stu-id="c6823-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="c6823-121">Représente l’heure de transition du jour et de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="c6823-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="c6823-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="c6823-123">Représente la _n_th occurrence du jour spécifiée dans l’élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) qui représente la date de transition de et de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="c6823-124">Month</span><span class="sxs-lookup"><span data-stu-id="c6823-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="c6823-125">Représente le mois de transition de l’année, de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="c6823-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="c6823-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="c6823-127">Représente le jour de la semaine où se produit la transition vers et à partir de l’heure et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="c6823-128">Année</span><span class="sxs-lookup"><span data-stu-id="c6823-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="c6823-129">Définit un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="c6823-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="c6823-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="c6823-130">This element is optional.</span></span> <span data-ttu-id="c6823-131">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c6823-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6823-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6823-132">Parent elements</span></span>

|<span data-ttu-id="c6823-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6823-133">**Element**</span></span>|<span data-ttu-id="c6823-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6823-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6823-135">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="c6823-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="c6823-136">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c6823-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="c6823-137">Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="c6823-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="c6823-138">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="c6823-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6823-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6823-139">Remarks</span></span>

<span data-ttu-id="c6823-140">L’élément **StandardTime Element** représente un temps de décalage représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="c6823-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="c6823-141">Lorsque l’élément de [polarisation](bias.md) enfant est égal à 0, l’heure standard est égale à l’offset de décalage par rapport à l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="c6823-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="c6823-142">Exemple</span><span class="sxs-lookup"><span data-stu-id="c6823-142">Example</span></span>

<span data-ttu-id="c6823-143">L’exemple suivant montre une région où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="c6823-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="c6823-144">La transition entre l’heure d’été et l’heure standard est observée à 2 h 00.</span><span class="sxs-lookup"><span data-stu-id="c6823-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="c6823-145">le cinquième dimanche du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="c6823-145">on the fifth Sunday of the tenth month.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="c6823-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6823-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6823-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6823-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6823-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6823-148">Schema Name</span></span>  <br/> |<span data-ttu-id="c6823-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c6823-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6823-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6823-150">Validation File</span></span>  <br/> |<span data-ttu-id="c6823-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c6823-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6823-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6823-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6823-153">False</span><span class="sxs-lookup"><span data-stu-id="c6823-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6823-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6823-154">See also</span></span>

- [<span data-ttu-id="c6823-155">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c6823-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c6823-156">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c6823-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

