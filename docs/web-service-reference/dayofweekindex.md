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
description: L’élément DayOfWeekIndex décrit quelle semaine d’un mois est utilisée dans une périodicité relative.
ms.openlocfilehash: c9235d83a944f9c8883439dd2adf190b88977f16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529209"
---
# <a name="dayofweekindex"></a><span data-ttu-id="fb564-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="fb564-103">DayOfWeekIndex</span></span>

<span data-ttu-id="fb564-104">L’élément **DayOfWeekIndex** décrit quelle semaine d’un mois est utilisée dans une périodicité relative.</span><span class="sxs-lookup"><span data-stu-id="fb564-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="fb564-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="fb564-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fb564-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb564-106">Attributes and elements</span></span>

<span data-ttu-id="fb564-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb564-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb564-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb564-108">Attributes</span></span>

<span data-ttu-id="fb564-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fb564-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb564-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb564-110">Child elements</span></span>

<span data-ttu-id="fb564-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb564-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb564-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb564-112">Parent elements</span></span>

|<span data-ttu-id="fb564-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb564-113">**Element**</span></span>|<span data-ttu-id="fb564-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb564-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb564-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="fb564-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="fb564-116">Décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="fb564-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="fb564-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="fb564-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="fb564-118">Décrit une périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="fb564-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb564-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="fb564-119">Text value</span></span>

<span data-ttu-id="fb564-120">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="fb564-120">A text value is required.</span></span> <span data-ttu-id="fb564-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="fb564-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="fb564-122">Premier</span><span class="sxs-lookup"><span data-stu-id="fb564-122">First</span></span>    
- <span data-ttu-id="fb564-123">Deuxième</span><span class="sxs-lookup"><span data-stu-id="fb564-123">Second</span></span>    
- <span data-ttu-id="fb564-124">Troisième</span><span class="sxs-lookup"><span data-stu-id="fb564-124">Third</span></span>    
- <span data-ttu-id="fb564-125">Quatrième</span><span class="sxs-lookup"><span data-stu-id="fb564-125">Fourth</span></span>    
- <span data-ttu-id="fb564-126">Nom</span><span class="sxs-lookup"><span data-stu-id="fb564-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fb564-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb564-127">Remarks</span></span>

<span data-ttu-id="fb564-128">Par exemple, le deuxième lundi d’un mois peut se produire dans la troisième semaine de ce mois.</span><span class="sxs-lookup"><span data-stu-id="fb564-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="fb564-129">Si un mois commence un vendredi, la première semaine du mois ne contient que quelques jours et ne contient pas de lundi.</span><span class="sxs-lookup"><span data-stu-id="fb564-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="fb564-130">Par conséquent, le premier lundi doit se produire dans la deuxième semaine.</span><span class="sxs-lookup"><span data-stu-id="fb564-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="fb564-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fb564-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb564-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb564-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb564-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb564-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb564-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb564-134">Schema name</span></span>  <br/> |<span data-ttu-id="fb564-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fb564-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb564-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb564-136">Validation file</span></span>  <br/> |<span data-ttu-id="fb564-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb564-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb564-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb564-138">Can be empty</span></span>  <br/> |<span data-ttu-id="fb564-139">False</span><span class="sxs-lookup"><span data-stu-id="fb564-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb564-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb564-140">See also</span></span>

- [<span data-ttu-id="fb564-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fb564-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

