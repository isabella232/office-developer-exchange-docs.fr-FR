---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: L’élément DayOfWeek représente le jour de la semaine où la transition de fuseau horaire a lieu.
ms.openlocfilehash: 7bc05f417268ccfb20adae12e2694d8360023ab2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457843"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="1a88e-103">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="1a88e-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="1a88e-104">L’élément **DayOfWeek** représente le jour de la semaine où la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="1a88e-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="1a88e-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="1a88e-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1a88e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a88e-106">Attributes and elements</span></span>

<span data-ttu-id="1a88e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a88e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a88e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a88e-108">Attributes</span></span>

<span data-ttu-id="1a88e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1a88e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a88e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a88e-110">Child elements</span></span>

<span data-ttu-id="1a88e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a88e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a88e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a88e-112">Parent elements</span></span>

|<span data-ttu-id="1a88e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a88e-113">**Element**</span></span>|<span data-ttu-id="1a88e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a88e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a88e-115">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="1a88e-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="1a88e-116">Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="1a88e-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="1a88e-117">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="1a88e-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="1a88e-118">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="1a88e-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="1a88e-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="1a88e-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="1a88e-120">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="1a88e-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="1a88e-121">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="1a88e-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="1a88e-122">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="1a88e-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="1a88e-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="1a88e-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="1a88e-124">Représente une transition de fuseau horaire qui se produit chaque année.</span><span class="sxs-lookup"><span data-stu-id="1a88e-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a88e-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1a88e-125">Text value</span></span>

<span data-ttu-id="1a88e-126">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="1a88e-126">A text value is required.</span></span> <span data-ttu-id="1a88e-127">La valeur de texte est représentée par une énumération qui a les valeurs possibles suivantes :</span><span class="sxs-lookup"><span data-stu-id="1a88e-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="1a88e-128">Warm</span><span class="sxs-lookup"><span data-stu-id="1a88e-128">Sunday</span></span>    
- <span data-ttu-id="1a88e-129">Lundi</span><span class="sxs-lookup"><span data-stu-id="1a88e-129">Monday</span></span>    
- <span data-ttu-id="1a88e-130">Mardi</span><span class="sxs-lookup"><span data-stu-id="1a88e-130">Tuesday</span></span>    
- <span data-ttu-id="1a88e-131">Mercredi</span><span class="sxs-lookup"><span data-stu-id="1a88e-131">Wednesday</span></span>    
- <span data-ttu-id="1a88e-132">Jeudi</span><span class="sxs-lookup"><span data-stu-id="1a88e-132">Thursday</span></span>    
- <span data-ttu-id="1a88e-133">Vendredi</span><span class="sxs-lookup"><span data-stu-id="1a88e-133">Friday</span></span>    
- <span data-ttu-id="1a88e-134">Samedi</span><span class="sxs-lookup"><span data-stu-id="1a88e-134">Saturday</span></span>    
- <span data-ttu-id="1a88e-135">Day</span><span class="sxs-lookup"><span data-stu-id="1a88e-135">Day</span></span>    
- <span data-ttu-id="1a88e-136">Jour de la semaine</span><span class="sxs-lookup"><span data-stu-id="1a88e-136">Weekday</span></span>   
- <span data-ttu-id="1a88e-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="1a88e-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1a88e-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="1a88e-138">Remarks</span></span>

<span data-ttu-id="1a88e-139">Un élément [StandardTime Element](standardtime.md) qui contient un élément [DayOrder](dayorder.md) ayant une valeur de 5, un élément [Month](month.md) qui a la valeur 10 et un élément **DayOfWeek** dont la valeur est dimanche signifie que la transition entre l’heure standard et l’heure d’été se produit le cinquième dimanche du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="1a88e-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="1a88e-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a88e-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a88e-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1a88e-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a88e-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1a88e-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a88e-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1a88e-143">Schema Name</span></span>  <br/> |<span data-ttu-id="1a88e-144">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1a88e-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a88e-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1a88e-145">Validation File</span></span>  <br/> |<span data-ttu-id="1a88e-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a88e-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a88e-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1a88e-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a88e-148">False</span><span class="sxs-lookup"><span data-stu-id="1a88e-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a88e-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a88e-149">See also</span></span>

- [<span data-ttu-id="1a88e-150">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1a88e-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="1a88e-151">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1a88e-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

