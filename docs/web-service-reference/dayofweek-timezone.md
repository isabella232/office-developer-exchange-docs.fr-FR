---
title: DayOfWeek (fuseau horaire)
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
description: L’élément DayOfWeek représente le jour de la semaine sur lequel se produit la transition de fuseau horaire.
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755819"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="2cfd4-103">DayOfWeek (fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="2cfd4-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="2cfd4-104">L’élément **DayOfWeek** représente le jour de la semaine sur lequel se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="2cfd4-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="2cfd4-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2cfd4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2cfd4-106">Attributes and elements</span></span>

<span data-ttu-id="2cfd4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cfd4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2cfd4-108">Attributes</span></span>

<span data-ttu-id="2cfd4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cfd4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2cfd4-110">Child elements</span></span>

<span data-ttu-id="2cfd4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2cfd4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2cfd4-112">Parent elements</span></span>

|<span data-ttu-id="2cfd4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2cfd4-113">**Element**</span></span>|<span data-ttu-id="2cfd4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2cfd4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cfd4-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="2cfd4-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="2cfd4-116">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="2cfd4-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="2cfd4-117">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="2cfd4-118">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="2cfd4-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="2cfd4-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="2cfd4-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="2cfd4-120">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="2cfd4-121">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="2cfd4-122">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="2cfd4-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="2cfd4-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="2cfd4-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="2cfd4-124">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2cfd4-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2cfd4-125">Text value</span></span>

<span data-ttu-id="2cfd4-126">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-126">A text value is required.</span></span> <span data-ttu-id="2cfd4-127">La valeur de texte est représentée par une énumération dont les valeurs possibles suivantes :</span><span class="sxs-lookup"><span data-stu-id="2cfd4-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="2cfd4-128">Dimanche</span><span class="sxs-lookup"><span data-stu-id="2cfd4-128">Sunday</span></span>    
- <span data-ttu-id="2cfd4-129">Lundi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-129">Monday</span></span>    
- <span data-ttu-id="2cfd4-130">Mardi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-130">Tuesday</span></span>    
- <span data-ttu-id="2cfd4-131">Mercredi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-131">Wednesday</span></span>    
- <span data-ttu-id="2cfd4-132">Jeudi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-132">Thursday</span></span>    
- <span data-ttu-id="2cfd4-133">Vendredi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-133">Friday</span></span>    
- <span data-ttu-id="2cfd4-134">Samedi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-134">Saturday</span></span>    
- <span data-ttu-id="2cfd4-135">Jour</span><span class="sxs-lookup"><span data-stu-id="2cfd4-135">Day</span></span>    
- <span data-ttu-id="2cfd4-136">Jour de la semaine</span><span class="sxs-lookup"><span data-stu-id="2cfd4-136">Weekday</span></span>   
- <span data-ttu-id="2cfd4-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="2cfd4-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2cfd4-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="2cfd4-138">Remarks</span></span>

<span data-ttu-id="2cfd4-139">Un élément [StandardTime](standardtime.md) qui contient un élément [DayOrder](dayorder.md) qui a une valeur de 5, un élément [mois](month.md) qui a une valeur de 10 et un élément **DayOfWeek** qui a une valeur de dimanche signifie que la transition d’heure standard à l’heure d’été gain de temps se produit le dimanche cinquième du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="2cfd4-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cfd4-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cfd4-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2cfd4-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cfd4-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2cfd4-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cfd4-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2cfd4-143">Schema Name</span></span>  <br/> |<span data-ttu-id="2cfd4-144">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2cfd4-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cfd4-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2cfd4-145">Validation File</span></span>  <br/> |<span data-ttu-id="2cfd4-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2cfd4-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cfd4-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2cfd4-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cfd4-148">False</span><span class="sxs-lookup"><span data-stu-id="2cfd4-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cfd4-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2cfd4-149">See also</span></span>

- [<span data-ttu-id="2cfd4-150">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2cfd4-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="2cfd4-151">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="2cfd4-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

