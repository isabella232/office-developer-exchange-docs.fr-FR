---
title: Point
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: L’élément period définit le nom, le décalage temporel et l’identificateur unique pour une étape spécifique du fuseau horaire.
ms.openlocfilehash: a7c36a9de01fd0484a7df75de3b5525992ef7ee7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459720"
---
# <a name="period"></a><span data-ttu-id="79cac-103">Point</span><span class="sxs-lookup"><span data-stu-id="79cac-103">Period</span></span>

<span data-ttu-id="79cac-104">L’élément **period** définit le nom, le décalage temporel et l’identificateur unique pour une étape spécifique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="79cac-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="79cac-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="79cac-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79cac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79cac-106">Attributes and elements</span></span>

<span data-ttu-id="79cac-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79cac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79cac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79cac-108">Attributes</span></span>

|<span data-ttu-id="79cac-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="79cac-109">**Attribute**</span></span>|<span data-ttu-id="79cac-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="79cac-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79cac-111">Bias</span><span class="sxs-lookup"><span data-stu-id="79cac-111">Bias</span></span>  <br/> |<span data-ttu-id="79cac-112">Valeur XS : Duration qui représente le décalage horaire par rapport au temps universel coordonné (UTC) pour la période.</span><span class="sxs-lookup"><span data-stu-id="79cac-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="79cac-113">Nom</span><span class="sxs-lookup"><span data-stu-id="79cac-113">Name</span></span>  <br/> |<span data-ttu-id="79cac-114">Valeur de type String qui représente le nom descriptif de la période.</span><span class="sxs-lookup"><span data-stu-id="79cac-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="79cac-115">ID</span><span class="sxs-lookup"><span data-stu-id="79cac-115">Id</span></span>  <br/> |<span data-ttu-id="79cac-116">Valeur de type String qui représente l’identificateur de la période.</span><span class="sxs-lookup"><span data-stu-id="79cac-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="79cac-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79cac-117">Child elements</span></span>

<span data-ttu-id="79cac-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79cac-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79cac-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79cac-119">Parent elements</span></span>

|<span data-ttu-id="79cac-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79cac-120">**Element**</span></span>|<span data-ttu-id="79cac-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="79cac-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79cac-122">Periods</span><span class="sxs-lookup"><span data-stu-id="79cac-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="79cac-123">Représente un tableau de périodes qui définissent le décalage temporel à différentes étapes du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="79cac-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79cac-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="79cac-124">Text value</span></span>

<span data-ttu-id="79cac-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79cac-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79cac-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="79cac-126">Remarks</span></span>

<span data-ttu-id="79cac-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79cac-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79cac-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79cac-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79cac-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79cac-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79cac-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79cac-130">Schema Name</span></span>  <br/> |<span data-ttu-id="79cac-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="79cac-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="79cac-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79cac-132">Validation File</span></span>  <br/> |<span data-ttu-id="79cac-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79cac-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79cac-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79cac-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="79cac-135">False</span><span class="sxs-lookup"><span data-stu-id="79cac-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79cac-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79cac-136">See also</span></span>



- [<span data-ttu-id="79cac-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79cac-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

