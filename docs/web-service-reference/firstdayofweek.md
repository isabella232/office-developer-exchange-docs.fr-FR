---
title: Premierjoursem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: L’élément FirstDayOfWeek spécifie le premier jour de la semaine.
ms.openlocfilehash: 1b4aee8e1ce2548cd6b0047623b0bcda47ad316b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530971"
---
# <a name="firstdayofweek"></a><span data-ttu-id="9e1ad-103">Premierjoursem</span><span class="sxs-lookup"><span data-stu-id="9e1ad-103">FirstDayOfWeek</span></span>

<span data-ttu-id="9e1ad-104">L’élément **FirstDayOfWeek** spécifie le premier jour de la semaine.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="9e1ad-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="9e1ad-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e1ad-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9e1ad-106">Attributes and elements</span></span>

<span data-ttu-id="9e1ad-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e1ad-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9e1ad-108">Attributes</span></span>

<span data-ttu-id="9e1ad-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e1ad-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9e1ad-110">Child elements</span></span>

<span data-ttu-id="9e1ad-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e1ad-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9e1ad-112">Parent elements</span></span>

|<span data-ttu-id="9e1ad-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e1ad-113">**Element**</span></span>|<span data-ttu-id="9e1ad-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e1ad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e1ad-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9e1ad-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="9e1ad-116">Décrit une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e1ad-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9e1ad-117">Text value</span></span>

<span data-ttu-id="9e1ad-118">La valeur de texte de l’élément **FirstDayOfWeek** indique le jour de la semaine utilisé comme premier jour de la semaine.</span><span class="sxs-lookup"><span data-stu-id="9e1ad-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="9e1ad-119">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="9e1ad-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="9e1ad-120">Warm</span><span class="sxs-lookup"><span data-stu-id="9e1ad-120">Sunday</span></span>
    
- <span data-ttu-id="9e1ad-121">Lundi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-121">Monday</span></span>
    
- <span data-ttu-id="9e1ad-122">Mardi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-122">Tuesday</span></span>
    
- <span data-ttu-id="9e1ad-123">Mercredi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-123">Wednesday</span></span>
    
- <span data-ttu-id="9e1ad-124">Jeudi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-124">Thursday</span></span>
    
- <span data-ttu-id="9e1ad-125">Vendredi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-125">Friday</span></span>
    
- <span data-ttu-id="9e1ad-126">Samedi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="9e1ad-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="9e1ad-127">Remarks</span></span>

<span data-ttu-id="9e1ad-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9e1ad-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e1ad-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9e1ad-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e1ad-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9e1ad-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e1ad-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9e1ad-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9e1ad-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9e1ad-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e1ad-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9e1ad-133">Validation File</span></span>  <br/> |<span data-ttu-id="9e1ad-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e1ad-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e1ad-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9e1ad-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e1ad-136">False</span><span class="sxs-lookup"><span data-stu-id="9e1ad-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e1ad-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9e1ad-137">See also</span></span>



- [<span data-ttu-id="9e1ad-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9e1ad-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

