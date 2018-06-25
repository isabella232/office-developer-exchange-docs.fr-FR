---
title: Mois
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
description: L’élément Month représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828476"
---
# <a name="month"></a><span data-ttu-id="a79a3-103">Mois</span><span class="sxs-lookup"><span data-stu-id="a79a3-103">Month</span></span>

<span data-ttu-id="a79a3-104">L’élément **Month** représente le mois de la transition de l’année vers et depuis l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="a79a3-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="a79a3-105">**Court**</span><span class="sxs-lookup"><span data-stu-id="a79a3-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a79a3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a79a3-106">Attributes and elements</span></span>

<span data-ttu-id="a79a3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a79a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a79a3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a79a3-108">Attributes</span></span>

<span data-ttu-id="a79a3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a79a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a79a3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a79a3-110">Child elements</span></span>

<span data-ttu-id="a79a3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a79a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a79a3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a79a3-112">Parent elements</span></span>

|<span data-ttu-id="a79a3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a79a3-113">**Element**</span></span>|<span data-ttu-id="a79a3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a79a3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a79a3-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="a79a3-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="a79a3-116">Représente un décalage de l’heure par rapport à temps universel coordonné (UTC) représenté par l’élément [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="a79a3-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="a79a3-117">Cet élément contient également des informations sur la transition à l’heure standard de l’heure dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="a79a3-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="a79a3-118">Les expressions XPath à l’élément [StandardTime](standardtime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a79a3-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="a79a3-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="a79a3-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="a79a3-120">Représente un décalage de l’heure par rapport à l’heure UTC représentée par l’élément [Bias (UTC)](bias-utc.md) dans les zones où l’heure d’été est respectée.</span><span class="sxs-lookup"><span data-stu-id="a79a3-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="a79a3-121">Cet élément contient également des informations sur la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="a79a3-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="a79a3-122">Les expressions XPath à l’élément [DaylightTime](daylighttime.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a79a3-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a79a3-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a79a3-123">Text value</span></span>

<span data-ttu-id="a79a3-124">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="a79a3-124">A text value is required.</span></span> <span data-ttu-id="a79a3-125">La valeur représente le rang ordinal du mois par occurrence et doit être un nombre compris entre 1 et 12.</span><span class="sxs-lookup"><span data-stu-id="a79a3-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="a79a3-126">Il s’agit d’un type de données entier court.</span><span class="sxs-lookup"><span data-stu-id="a79a3-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a79a3-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="a79a3-127">Remarks</span></span>

<span data-ttu-id="a79a3-128">Un élément [StandardTime](standardtime.md) qui contient un élément [DayOrder](dayorder.md) qui a une valeur de 5, un élément **mois** qui a une valeur de 10 et un élément [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) qui a une valeur de dimanche signifie que la transition à partir de l’heure l’heure d’été se produit le dimanche cinquième du dixième mois.</span><span class="sxs-lookup"><span data-stu-id="a79a3-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a79a3-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a79a3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a79a3-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a79a3-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a79a3-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a79a3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a79a3-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a79a3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a79a3-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a79a3-133">Validation File</span></span>  <br/> |<span data-ttu-id="a79a3-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a79a3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a79a3-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a79a3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a79a3-136">False</span><span class="sxs-lookup"><span data-stu-id="a79a3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a79a3-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a79a3-137">See also</span></span>

- [<span data-ttu-id="a79a3-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a79a3-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a79a3-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a79a3-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

