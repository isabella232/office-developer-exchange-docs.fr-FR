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
description: L’élément Period définit le nom, le décalage et l’identificateur unique pour une étape spécifique du fuseau horaire.
ms.openlocfilehash: 3b5d5877e6d9baffdfe536a0feec3b25b6d2883f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828726"
---
# <a name="period"></a><span data-ttu-id="9811b-103">Point</span><span class="sxs-lookup"><span data-stu-id="9811b-103">Period</span></span>

<span data-ttu-id="9811b-104">L’élément **Period** définit le nom, le décalage et l’identificateur unique pour une étape spécifique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9811b-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="9811b-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="9811b-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9811b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9811b-106">Attributes and elements</span></span>

<span data-ttu-id="9811b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9811b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9811b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9811b-108">Attributes</span></span>

|<span data-ttu-id="9811b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9811b-109">**Attribute**</span></span>|<span data-ttu-id="9811b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9811b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9811b-111">Bias</span><span class="sxs-lookup"><span data-stu-id="9811b-111">Bias</span></span>  <br/> |<span data-ttu-id="9811b-112">Une valeur xs qui représente le décalage du temps universel coordonné (UTC) pour la période.</span><span class="sxs-lookup"><span data-stu-id="9811b-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="9811b-113">Nom</span><span class="sxs-lookup"><span data-stu-id="9811b-113">Name</span></span>  <br/> |<span data-ttu-id="9811b-114">Une valeur de type string qui représente le nom descriptif de la période.</span><span class="sxs-lookup"><span data-stu-id="9811b-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="9811b-115">ID</span><span class="sxs-lookup"><span data-stu-id="9811b-115">Id</span></span>  <br/> |<span data-ttu-id="9811b-116">Une valeur de type string qui représente l’identificateur pour la période.</span><span class="sxs-lookup"><span data-stu-id="9811b-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9811b-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9811b-117">Child elements</span></span>

<span data-ttu-id="9811b-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9811b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9811b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9811b-119">Parent elements</span></span>

|<span data-ttu-id="9811b-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9811b-120">**Element**</span></span>|<span data-ttu-id="9811b-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="9811b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9811b-122">Périodes</span><span class="sxs-lookup"><span data-stu-id="9811b-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="9811b-123">Représente un tableau de points qui définissent le décalage de temps à différents stades du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9811b-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9811b-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9811b-124">Text value</span></span>

<span data-ttu-id="9811b-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9811b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9811b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="9811b-126">Remarks</span></span>

<span data-ttu-id="9811b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9811b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9811b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9811b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9811b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9811b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9811b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9811b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9811b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9811b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="9811b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9811b-132">Validation File</span></span>  <br/> |<span data-ttu-id="9811b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9811b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9811b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9811b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9811b-135">False</span><span class="sxs-lookup"><span data-stu-id="9811b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9811b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9811b-136">See also</span></span>



- [<span data-ttu-id="9811b-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9811b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

