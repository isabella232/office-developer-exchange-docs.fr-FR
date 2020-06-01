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
description: L’élément Bias représente le décalage général par rapport au temps universel coordonné (UTC). Cette valeur est exprimée en minutes.
ms.openlocfilehash: d95284aa28e59542d1a1ee40686163138b015702
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460245"
---
# <a name="bias-utc"></a><span data-ttu-id="22f7b-104">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="22f7b-104">Bias (UTC)</span></span>

<span data-ttu-id="22f7b-105">L’élément **Bias** représente le décalage général par rapport au temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="22f7b-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="22f7b-106">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="22f7b-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="22f7b-107">**int**</span><span class="sxs-lookup"><span data-stu-id="22f7b-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="22f7b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22f7b-108">Attributes and elements</span></span>

<span data-ttu-id="22f7b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22f7b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22f7b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="22f7b-110">Attributes</span></span>

<span data-ttu-id="22f7b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22f7b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22f7b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22f7b-112">Child elements</span></span>

<span data-ttu-id="22f7b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22f7b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22f7b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22f7b-114">Parent elements</span></span>

|<span data-ttu-id="22f7b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22f7b-115">**Element**</span></span>|<span data-ttu-id="22f7b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="22f7b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22f7b-117">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="22f7b-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="22f7b-118">Conteneur qui identifie les informations de date et d’heure de la demande.</span><span class="sxs-lookup"><span data-stu-id="22f7b-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="22f7b-119">Cet élément contient des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="22f7b-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="22f7b-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="22f7b-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22f7b-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="22f7b-121">Text value</span></span>

<span data-ttu-id="22f7b-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="22f7b-122">A text value is required.</span></span> <span data-ttu-id="22f7b-123">La valeur texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="22f7b-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22f7b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="22f7b-124">Remarks</span></span>

<span data-ttu-id="22f7b-125">Un deuxième élément [Bias](bias.md) dans le schéma représente le décalage par rapport à l’offset UTC (temps universel coordonné).</span><span class="sxs-lookup"><span data-stu-id="22f7b-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="22f7b-126">Exemple</span><span class="sxs-lookup"><span data-stu-id="22f7b-126">Example</span></span>

<span data-ttu-id="22f7b-127">L’exemple suivant montre une partie d’une requête XML qui identifie un décalage de 8 heures par rapport à l’heure UTC sur l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="22f7b-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="22f7b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22f7b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22f7b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22f7b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22f7b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22f7b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="22f7b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="22f7b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="22f7b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22f7b-132">Validation File</span></span>  <br/> |<span data-ttu-id="22f7b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22f7b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22f7b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22f7b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="22f7b-135">False</span><span class="sxs-lookup"><span data-stu-id="22f7b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22f7b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22f7b-136">See also</span></span>

- [<span data-ttu-id="22f7b-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="22f7b-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="22f7b-138">Bias</span><span class="sxs-lookup"><span data-stu-id="22f7b-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="22f7b-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="22f7b-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

