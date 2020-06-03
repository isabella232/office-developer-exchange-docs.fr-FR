---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: L’élément month représente le mois de transition de l’année, de l’heure standard et de l’heure d’été.
ms.openlocfilehash: f102dca4ed9e833b9742844cfd612c81dfd05e70
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468620"
---
# <a name="month"></a><span data-ttu-id="2ea49-103">Month</span><span class="sxs-lookup"><span data-stu-id="2ea49-103">Month</span></span>

<span data-ttu-id="2ea49-104">L’élément **Month** représente le mois de transition de l’année, de l’heure standard et de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="2ea49-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="2ea49-105">**Inférieure**</span><span class="sxs-lookup"><span data-stu-id="2ea49-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ea49-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ea49-106">Attributes and elements</span></span>

<span data-ttu-id="2ea49-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ea49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ea49-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ea49-108">Attributes</span></span>

<span data-ttu-id="2ea49-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2ea49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ea49-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ea49-110">Child elements</span></span>

<span data-ttu-id="2ea49-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ea49-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ea49-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ea49-112">Parent elements</span></span>

|<span data-ttu-id="2ea49-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ea49-113">**Element**</span></span>|<span data-ttu-id="2ea49-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ea49-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ea49-115">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="2ea49-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="2ea49-116">Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="2ea49-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="2ea49-117">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="2ea49-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="2ea49-118">Voici les expressions XPath de l’élément [StandardTime Element](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="2ea49-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="2ea49-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="2ea49-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="2ea49-120">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="2ea49-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="2ea49-121">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="2ea49-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="2ea49-122">Voici les expressions XPath de l’élément [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="2ea49-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ea49-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2ea49-123">Text value</span></span>

<span data-ttu-id="2ea49-124">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="2ea49-124">A text value is required.</span></span> <span data-ttu-id="2ea49-125">La valeur représente le rang ordinal du mois par occurrence et doit être un nombre compris entre 1 et 12.</span><span class="sxs-lookup"><span data-stu-id="2ea49-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="2ea49-126">Il s’agit d’un type de données entier court.</span><span class="sxs-lookup"><span data-stu-id="2ea49-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ea49-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ea49-127">Remarks</span></span>

<span data-ttu-id="2ea49-128">Un élément [StandardTime Element](standardtime.md) qui contient un élément [DayOrder](dayorder.md) ayant la valeur 5, un élément **Month** qui a la valeur 10 et un élément [DayOfWeek (TimeZone)](dayofweek-timezone.md) ayant la valeur dimanche signifie que la transition entre l’heure standard et l’heure d’été a lieu le cinquième dimanche du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="2ea49-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2ea49-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ea49-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ea49-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ea49-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ea49-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ea49-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2ea49-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ea49-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ea49-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ea49-133">Validation File</span></span>  <br/> |<span data-ttu-id="2ea49-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ea49-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ea49-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ea49-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ea49-136">False</span><span class="sxs-lookup"><span data-stu-id="2ea49-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ea49-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ea49-137">See also</span></span>

- [<span data-ttu-id="2ea49-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2ea49-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="2ea49-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2ea49-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

