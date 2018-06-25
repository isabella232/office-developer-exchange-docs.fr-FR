---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: L’élément MergedFreeBusyIntervalInMinutes représente la différence entre deux emplacements successifs dans la vue FreeBusyMerged.
ms.openlocfilehash: 99c8c69424a0a9d9594005fdf6b2ceba53e6288a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828451"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="ba54e-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="ba54e-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="ba54e-104">L’élément **MergedFreeBusyIntervalInMinutes** représente la différence entre deux emplacements successifs dans la vue **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="ba54e-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="ba54e-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ba54e-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="ba54e-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="ba54e-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="ba54e-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="ba54e-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="ba54e-108">**int**</span><span class="sxs-lookup"><span data-stu-id="ba54e-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba54e-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba54e-109">Attributes and elements</span></span>

<span data-ttu-id="ba54e-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba54e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba54e-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba54e-111">Attributes</span></span>

<span data-ttu-id="ba54e-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba54e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba54e-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba54e-113">Child elements</span></span>

<span data-ttu-id="ba54e-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba54e-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba54e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba54e-115">Parent elements</span></span>

|<span data-ttu-id="ba54e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba54e-116">**Element**</span></span>|<span data-ttu-id="ba54e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba54e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba54e-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="ba54e-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="ba54e-119">Spécifie le type d’informations disponible/occupé retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ba54e-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="ba54e-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ba54e-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba54e-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ba54e-121">Text value</span></span>

<span data-ttu-id="ba54e-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="ba54e-122">A text value is required.</span></span> <span data-ttu-id="ba54e-123">La valeur de texte représente la durée en minutes.</span><span class="sxs-lookup"><span data-stu-id="ba54e-123">The text value represents time in minutes.</span></span> <span data-ttu-id="ba54e-124">La valeur par défaut est 30 minutes.</span><span class="sxs-lookup"><span data-stu-id="ba54e-124">The default value is 30 minutes.</span></span> <span data-ttu-id="ba54e-125">Six minutes est l’intervalle minimal et un jour (1 440 minutes) l’intervalle maximal de cet élément.</span><span class="sxs-lookup"><span data-stu-id="ba54e-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba54e-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba54e-126">Remarks</span></span>

<span data-ttu-id="ba54e-127">Cette valeur est utilisée uniquement si l’élément [RequestedView](requestedview.md) est égale à **MergedOnly**, **FreeBusyMerged**ou **DetailedMerge**.</span><span class="sxs-lookup"><span data-stu-id="ba54e-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="ba54e-128">Il s’agit d’un type de données integer.</span><span class="sxs-lookup"><span data-stu-id="ba54e-128">This is an integer data type.</span></span> <span data-ttu-id="ba54e-129">Flux qui contient les intervalles définis par cet élément est renvoyé dans l’élément [MergedFreeBusy](mergedfreebusy.md) .</span><span class="sxs-lookup"><span data-stu-id="ba54e-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ba54e-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba54e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba54e-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba54e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba54e-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba54e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ba54e-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ba54e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba54e-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba54e-134">Validation File</span></span>  <br/> |<span data-ttu-id="ba54e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba54e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba54e-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba54e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba54e-137">False</span><span class="sxs-lookup"><span data-stu-id="ba54e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba54e-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba54e-138">See also</span></span>



[<span data-ttu-id="ba54e-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ba54e-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ba54e-140">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ba54e-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="ba54e-141">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="ba54e-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

