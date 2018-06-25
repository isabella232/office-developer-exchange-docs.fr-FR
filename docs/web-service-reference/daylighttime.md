---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: L’élément DaylightTime représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément Bias (UTC) dans les zones où l’heure d’été est respectée. Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755818"
---
# <a name="daylighttime"></a><span data-ttu-id="7a2c1-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="7a2c1-104">DaylightTime</span></span>

<span data-ttu-id="7a2c1-105">L’élément **DaylightTime** représente un décalage de l’heure par rapport à temps universel coordonné (UTC) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="7a2c1-106">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="7a2c1-107">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="7a2c1-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="7a2c1-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="7a2c1-108">DaylightTime</span></span>](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

<span data-ttu-id="7a2c1-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="7a2c1-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7a2c1-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a2c1-110">Attributes and elements</span></span>

<span data-ttu-id="7a2c1-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a2c1-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a2c1-112">Attributes</span></span>

<span data-ttu-id="7a2c1-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a2c1-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a2c1-114">Child elements</span></span>

|<span data-ttu-id="7a2c1-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a2c1-115">**Element**</span></span>|<span data-ttu-id="7a2c1-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a2c1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a2c1-117">Bias</span><span class="sxs-lookup"><span data-stu-id="7a2c1-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="7a2c1-118">Représente le décalage de l’offset UTC identifié par l’élément [Bias (UTC)](bias-utc.md) heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="7a2c1-119">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="7a2c1-120">Heure</span><span class="sxs-lookup"><span data-stu-id="7a2c1-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="7a2c1-121">Représente le temps de transition de la journée à et d’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7a2c1-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="7a2c1-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="7a2c1-123">Représente l’occurrence _n_th de la journée qui est spécifiée dans l’élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui représente la date de transition d’et à l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7a2c1-124">Mois</span><span class="sxs-lookup"><span data-stu-id="7a2c1-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="7a2c1-125">Représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7a2c1-126">DayOfWeek (fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="7a2c1-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="7a2c1-127">Représente le jour de la semaine quand se produit la transition vers et depuis l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="7a2c1-128">Année</span><span class="sxs-lookup"><span data-stu-id="7a2c1-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="7a2c1-129">Utilisé pour définir un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="7a2c1-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-130">This element is optional.</span></span> <span data-ttu-id="7a2c1-131">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7a2c1-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a2c1-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a2c1-132">Parent elements</span></span>

|<span data-ttu-id="7a2c1-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a2c1-133">**Element**</span></span>|<span data-ttu-id="7a2c1-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a2c1-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a2c1-135">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="7a2c1-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="7a2c1-136">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="7a2c1-137">Cet élément contient également des informations sur la transition entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="7a2c1-138">Exemple</span><span class="sxs-lookup"><span data-stu-id="7a2c1-138">Example</span></span>

<span data-ttu-id="7a2c1-139">La demande GetUserAvailability partielle suivante représente une application cliente dans un emplacement qui reconnaît l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="7a2c1-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="7a2c1-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a2c1-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a2c1-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a2c1-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a2c1-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a2c1-142">Schema Name</span></span>  <br/> |<span data-ttu-id="7a2c1-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7a2c1-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a2c1-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7a2c1-144">Validation File</span></span>  <br/> |<span data-ttu-id="7a2c1-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a2c1-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a2c1-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a2c1-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a2c1-147">False</span><span class="sxs-lookup"><span data-stu-id="7a2c1-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a2c1-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a2c1-148">See also</span></span>

- [<span data-ttu-id="7a2c1-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7a2c1-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7a2c1-150">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="7a2c1-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

