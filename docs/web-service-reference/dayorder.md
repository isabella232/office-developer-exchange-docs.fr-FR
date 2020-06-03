---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: L’élément DayOrder représente la nième occurrence du jour spécifié dans l’élément DayOfWeek (TimeZone) qui représente la date de transition de l’heure standard à l’heure d’été et de l’heure d’été.
ms.openlocfilehash: 53a8cb979bdb7aefead5623b4680f4c1a4ef5509
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526962"
---
# <a name="dayorder"></a><span data-ttu-id="71ef8-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="71ef8-103">DayOrder</span></span>

<span data-ttu-id="71ef8-104">L’élément **DayOrder** représente le _n_th occurrence du jour spécifié dans l’élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) qui représente la date de transition de et vers l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="71ef8-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="71ef8-105">**inférieure**</span><span class="sxs-lookup"><span data-stu-id="71ef8-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="71ef8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71ef8-106">Attributes and elements</span></span>

<span data-ttu-id="71ef8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71ef8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71ef8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71ef8-108">Attributes</span></span>

<span data-ttu-id="71ef8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="71ef8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71ef8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71ef8-110">Child elements</span></span>

<span data-ttu-id="71ef8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71ef8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71ef8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71ef8-112">Parent elements</span></span>

|<span data-ttu-id="71ef8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71ef8-113">**Element**</span></span>|<span data-ttu-id="71ef8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="71ef8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71ef8-115">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="71ef8-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="71ef8-116">Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="71ef8-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="71ef8-117">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="71ef8-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="71ef8-118">Voici les expressions XPath de l’élément [StandardTime Element](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="71ef8-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="71ef8-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="71ef8-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="71ef8-120">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="71ef8-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="71ef8-121">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="71ef8-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="71ef8-122">Voici les expressions XPath de l’élément [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="71ef8-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71ef8-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="71ef8-123">Text value</span></span>

<span data-ttu-id="71ef8-124">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="71ef8-124">A text value is required.</span></span> <span data-ttu-id="71ef8-125">La valeur de l’élément **DayOrder** peut être comprise entre 1 et 5.</span><span class="sxs-lookup"><span data-stu-id="71ef8-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="71ef8-126">La valeur maximale de cet élément peut être 4 ou 5, selon le mois et l’année.</span><span class="sxs-lookup"><span data-stu-id="71ef8-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="71ef8-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="71ef8-127">Remarks</span></span>

<span data-ttu-id="71ef8-128">Un élément [StandardTime Element](standardtime.md) qui contient un élément **DayOrder** ayant la valeur 5, un élément [Month](month.md) qui a la valeur 10 et un élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) ayant la valeur dimanche signifie que la transition entre l’heure standard et l’heure d’été a lieu le cinquième dimanche du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="71ef8-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="71ef8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71ef8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71ef8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71ef8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71ef8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71ef8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="71ef8-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71ef8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="71ef8-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71ef8-133">Validation File</span></span>  <br/> |<span data-ttu-id="71ef8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71ef8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71ef8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71ef8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="71ef8-136">False</span><span class="sxs-lookup"><span data-stu-id="71ef8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71ef8-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71ef8-137">See also</span></span>

- [<span data-ttu-id="71ef8-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="71ef8-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="71ef8-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="71ef8-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

