---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: L’élément AbsoluteDateTransition représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.
ms.openlocfilehash: 1e9e5f3f2269814a82b827efe46c71a172e21348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755150"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="e2084-103">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="e2084-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="e2084-104">L’élément **AbsoluteDateTransition** représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.</span><span class="sxs-lookup"><span data-stu-id="e2084-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="e2084-105">**AbsoluteDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="e2084-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e2084-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e2084-106">Attributes and elements</span></span>

<span data-ttu-id="e2084-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e2084-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2084-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e2084-108">Attributes</span></span>

<span data-ttu-id="e2084-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e2084-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2084-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e2084-110">Child elements</span></span>

|<span data-ttu-id="e2084-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2084-111">**Element**</span></span>|<span data-ttu-id="e2084-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2084-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2084-113">Pour</span><span class="sxs-lookup"><span data-stu-id="e2084-113">To</span></span>](to.md) <br/> |<span data-ttu-id="e2084-114">Spécifie la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e2084-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="e2084-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="e2084-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="e2084-116">Représente la date et l’heure à laquelle se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e2084-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2084-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e2084-117">Parent elements</span></span>

|<span data-ttu-id="e2084-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2084-118">**Element**</span></span>|<span data-ttu-id="e2084-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2084-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2084-120">Transitions</span><span class="sxs-lookup"><span data-stu-id="e2084-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e2084-121">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e2084-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e2084-122">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="e2084-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="e2084-123">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e2084-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2084-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="e2084-124">Remarks</span></span>

<span data-ttu-id="e2084-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2084-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2084-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e2084-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2084-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e2084-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2084-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e2084-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e2084-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e2084-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2084-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e2084-130">Validation File</span></span>  <br/> |<span data-ttu-id="e2084-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2084-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2084-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e2084-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2084-133">False</span><span class="sxs-lookup"><span data-stu-id="e2084-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2084-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e2084-134">See also</span></span>

- [<span data-ttu-id="e2084-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e2084-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
