---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: L’élément DayOfWeekIndex décrit la semaine du mois est utilisée dans une périodicité relative.
ms.openlocfilehash: 4987685d0c3cefdfad4f5be1368776a5b859bf94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755825"
---
# <a name="dayofweekindex"></a><span data-ttu-id="63aa9-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="63aa9-103">DayOfWeekIndex</span></span>

<span data-ttu-id="63aa9-104">L’élément **DayOfWeekIndex** décrit la semaine du mois est utilisée dans une périodicité relative.</span><span class="sxs-lookup"><span data-stu-id="63aa9-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="63aa9-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="63aa9-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63aa9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63aa9-106">Attributes and elements</span></span>

<span data-ttu-id="63aa9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63aa9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63aa9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="63aa9-108">Attributes</span></span>

<span data-ttu-id="63aa9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63aa9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63aa9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63aa9-110">Child elements</span></span>

<span data-ttu-id="63aa9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63aa9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63aa9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63aa9-112">Parent elements</span></span>

|<span data-ttu-id="63aa9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63aa9-113">**Element**</span></span>|<span data-ttu-id="63aa9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="63aa9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63aa9-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="63aa9-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="63aa9-116">Décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="63aa9-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="63aa9-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="63aa9-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="63aa9-118">Décrit une périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="63aa9-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63aa9-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="63aa9-119">Text value</span></span>

<span data-ttu-id="63aa9-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="63aa9-120">A text value is required.</span></span> <span data-ttu-id="63aa9-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="63aa9-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="63aa9-122">Première</span><span class="sxs-lookup"><span data-stu-id="63aa9-122">First</span></span>    
- <span data-ttu-id="63aa9-123">Deuxième</span><span class="sxs-lookup"><span data-stu-id="63aa9-123">Second</span></span>    
- <span data-ttu-id="63aa9-124">Troisième</span><span class="sxs-lookup"><span data-stu-id="63aa9-124">Third</span></span>    
- <span data-ttu-id="63aa9-125">Quatrième</span><span class="sxs-lookup"><span data-stu-id="63aa9-125">Fourth</span></span>    
- <span data-ttu-id="63aa9-126">Last</span><span class="sxs-lookup"><span data-stu-id="63aa9-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="63aa9-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="63aa9-127">Remarks</span></span>

<span data-ttu-id="63aa9-128">Par exemple, le deuxième lundi du mois peut se produire dans la troisième semaine du mois.</span><span class="sxs-lookup"><span data-stu-id="63aa9-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="63aa9-129">Si un mois commence un vendredi, la première semaine du mois contient quelques jours uniquement et ne contient-elle pas un lundi.</span><span class="sxs-lookup"><span data-stu-id="63aa9-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="63aa9-130">Par conséquent, le premier lundi doit se produire dans la deuxième semaine.</span><span class="sxs-lookup"><span data-stu-id="63aa9-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="63aa9-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="63aa9-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63aa9-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63aa9-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63aa9-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63aa9-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63aa9-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63aa9-134">Schema name</span></span>  <br/> |<span data-ttu-id="63aa9-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="63aa9-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="63aa9-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63aa9-136">Validation file</span></span>  <br/> |<span data-ttu-id="63aa9-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63aa9-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63aa9-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63aa9-138">Can be empty</span></span>  <br/> |<span data-ttu-id="63aa9-139">False</span><span class="sxs-lookup"><span data-stu-id="63aa9-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63aa9-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63aa9-140">See also</span></span>

- [<span data-ttu-id="63aa9-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63aa9-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

