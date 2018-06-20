---
title: Bias (UTC)
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
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: L’élément Bias représente le décalage général du temps universel coordonné (UTC). Cette valeur est exprimée en minutes.
ms.openlocfilehash: 43613593565ca15be97bd2a98dbe5c512dbe5fc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755385"
---
# <a name="bias-utc"></a><span data-ttu-id="2d318-104">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="2d318-104">Bias (UTC)</span></span>

<span data-ttu-id="2d318-105">L’élément **Bias** représente le décalage général du temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="2d318-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="2d318-106">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="2d318-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="2d318-107">**int**</span><span class="sxs-lookup"><span data-stu-id="2d318-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2d318-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d318-108">Attributes and elements</span></span>

<span data-ttu-id="2d318-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d318-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d318-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d318-110">Attributes</span></span>

<span data-ttu-id="2d318-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d318-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d318-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d318-112">Child elements</span></span>

<span data-ttu-id="2d318-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d318-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d318-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d318-114">Parent elements</span></span>

|<span data-ttu-id="2d318-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d318-115">**Element**</span></span>|<span data-ttu-id="2d318-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d318-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d318-117">Fuseau horaire (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="2d318-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="2d318-118">Conteneur qui identifie les informations de date et heure de la demande.</span><span class="sxs-lookup"><span data-stu-id="2d318-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="2d318-119">Cet élément contient des informations sur la transition entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="2d318-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="2d318-120">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="2d318-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d318-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2d318-121">Text value</span></span>

<span data-ttu-id="2d318-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="2d318-122">A text value is required.</span></span> <span data-ttu-id="2d318-123">La valeur de texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="2d318-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2d318-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d318-124">Remarks</span></span>

<span data-ttu-id="2d318-125">Un deuxième élément [Bias](bias.md) dans le schéma représente le décalage de l’offset de temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="2d318-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="2d318-126">Exemple</span><span class="sxs-lookup"><span data-stu-id="2d318-126">Example</span></span>

<span data-ttu-id="2d318-127">L’exemple suivant montre une partie d’une requête XML qui identifie un décalage de 8 heures à l’heure UTC dans l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="2d318-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="2d318-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d318-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d318-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d318-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d318-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d318-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2d318-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2d318-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d318-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d318-132">Validation File</span></span>  <br/> |<span data-ttu-id="2d318-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d318-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d318-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d318-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d318-135">False</span><span class="sxs-lookup"><span data-stu-id="2d318-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d318-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d318-136">See also</span></span>

- [<span data-ttu-id="2d318-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2d318-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="2d318-138">Bias</span><span class="sxs-lookup"><span data-stu-id="2d318-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="2d318-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="2d318-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

