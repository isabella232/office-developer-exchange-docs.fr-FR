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
description: L’élément DaylightTime représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément bias (UTC) dans les régions où l’heure d’été est observée. Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.
ms.openlocfilehash: 350fcb4ce278f423c62fcc5ecaa160eda71e4a2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455652"
---
# <a name="daylighttime"></a><span data-ttu-id="9d194-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="9d194-104">DaylightTime</span></span>

<span data-ttu-id="9d194-105">L’élément **DaylightTime** représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="9d194-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="9d194-106">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="9d194-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="9d194-107">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="9d194-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="9d194-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="9d194-108">DaylightTime</span></span>](daylighttime.md)
  
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

<span data-ttu-id="9d194-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="9d194-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9d194-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9d194-110">Attributes and elements</span></span>

<span data-ttu-id="9d194-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9d194-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d194-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="9d194-112">Attributes</span></span>

<span data-ttu-id="9d194-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9d194-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d194-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9d194-114">Child elements</span></span>

|<span data-ttu-id="9d194-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d194-115">**Element**</span></span>|<span data-ttu-id="9d194-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d194-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d194-117">Bias</span><span class="sxs-lookup"><span data-stu-id="9d194-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="9d194-118">Représente le décalage à partir de l’offset UTC identifié par l’élément [bias (UTC)](bias-utc.md) pour l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="9d194-119">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="9d194-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="9d194-120">Time</span><span class="sxs-lookup"><span data-stu-id="9d194-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="9d194-121">Représente l’heure de transition du jour et de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="9d194-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="9d194-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="9d194-123">Représente la _n_th occurrence du jour spécifiée dans l’élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) qui représente la date de transition de et de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="9d194-124">Month</span><span class="sxs-lookup"><span data-stu-id="9d194-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="9d194-125">Représente le mois de transition de l’année, de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="9d194-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="9d194-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="9d194-127">Représente le jour de la semaine où se produit la transition vers et à partir de l’heure et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="9d194-128">Année</span><span class="sxs-lookup"><span data-stu-id="9d194-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="9d194-129">Permet de définir un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="9d194-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="9d194-130">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9d194-130">This element is optional.</span></span> <span data-ttu-id="9d194-131">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9d194-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d194-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9d194-132">Parent elements</span></span>

|<span data-ttu-id="9d194-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d194-133">**Element**</span></span>|<span data-ttu-id="9d194-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d194-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d194-135">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="9d194-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="9d194-136">Contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9d194-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="9d194-137">Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="9d194-138">Exemple</span><span class="sxs-lookup"><span data-stu-id="9d194-138">Example</span></span>

<span data-ttu-id="9d194-139">La requête GetUserAvailability partielle suivante représente une application cliente dans un emplacement qui reconnaît l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="9d194-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="9d194-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9d194-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d194-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9d194-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d194-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9d194-142">Schema Name</span></span>  <br/> |<span data-ttu-id="9d194-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9d194-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d194-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9d194-144">Validation File</span></span>  <br/> |<span data-ttu-id="9d194-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d194-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d194-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9d194-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d194-147">False</span><span class="sxs-lookup"><span data-stu-id="9d194-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d194-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9d194-148">See also</span></span>

- [<span data-ttu-id="9d194-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9d194-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="9d194-150">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9d194-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

