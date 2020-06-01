---
title: Year
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: L’élément Year est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: cc83f9b2137f151f3f8ef0ceaf603ec036989961
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465169"
---
# <a name="year"></a><span data-ttu-id="2de56-105">Year</span><span class="sxs-lookup"><span data-stu-id="2de56-105">Year</span></span>

<span data-ttu-id="2de56-106">L’élément **year** est utilisé pour définir un fuseau horaire qui change en fonction de l’année.</span><span class="sxs-lookup"><span data-stu-id="2de56-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="2de56-107">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="2de56-107">This element is optional.</span></span> <span data-ttu-id="2de56-108">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2de56-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="2de56-109">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="2de56-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2de56-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2de56-110">Attributes and elements</span></span>

<span data-ttu-id="2de56-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2de56-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2de56-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="2de56-112">Attributes</span></span>

<span data-ttu-id="2de56-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2de56-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2de56-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2de56-114">Child elements</span></span>

<span data-ttu-id="2de56-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2de56-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2de56-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2de56-116">Parent elements</span></span>

|<span data-ttu-id="2de56-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2de56-117">**Element**</span></span>|<span data-ttu-id="2de56-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="2de56-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2de56-119">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="2de56-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="2de56-120">Représente un décalage entre l’heure par rapport à l’heure UTC (Coordinated Universal Time) représentée par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="2de56-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="2de56-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="2de56-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="2de56-122">Représente un décalage entre l’heure par rapport à l’heure UTC (Coordinated Universal Time) représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="2de56-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2de56-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2de56-123">Text value</span></span>

<span data-ttu-id="2de56-124">L’élément Year accepte une chaîne qui représente une année.</span><span class="sxs-lookup"><span data-stu-id="2de56-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="2de56-125">Le format de l’année est YYYY.</span><span class="sxs-lookup"><span data-stu-id="2de56-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2de56-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2de56-126">Remarks</span></span>

<span data-ttu-id="2de56-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2de56-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2de56-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2de56-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2de56-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2de56-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2de56-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2de56-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2de56-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2de56-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2de56-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2de56-132">Validation File</span></span>  <br/> |<span data-ttu-id="2de56-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2de56-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2de56-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2de56-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2de56-135">False</span><span class="sxs-lookup"><span data-stu-id="2de56-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2de56-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2de56-136">See also</span></span>

- [<span data-ttu-id="2de56-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2de56-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

