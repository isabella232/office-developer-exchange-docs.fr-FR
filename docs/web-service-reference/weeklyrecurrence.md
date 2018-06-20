---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: L’élément WeeklyRecurrence décrit une périodicité hebdomadaire.
ms.openlocfilehash: 78bc76dd63c6737786df02f336217dc8de9a3a67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839041"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="7e304-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="7e304-103">WeeklyRecurrence</span></span>

<span data-ttu-id="7e304-104">L’élément **WeeklyRecurrence** décrit une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="7e304-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="7e304-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="7e304-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e304-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7e304-106">Attributes and elements</span></span>

<span data-ttu-id="7e304-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7e304-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e304-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7e304-108">Attributes</span></span>

<span data-ttu-id="7e304-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e304-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e304-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7e304-110">Child elements</span></span>

|<span data-ttu-id="7e304-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7e304-111">**Element**</span></span>|<span data-ttu-id="7e304-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7e304-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e304-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="7e304-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7e304-114">Définit l’intervalle, en semaines, entre deux consécutifs hebdomadaire périodicité éléments du modèle.</span><span class="sxs-lookup"><span data-stu-id="7e304-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="7e304-115">La valeur peut être compris entre 1 et 99.</span><span class="sxs-lookup"><span data-stu-id="7e304-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="7e304-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="7e304-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="7e304-117">Décrit les jours de la semaine dans la périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="7e304-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="7e304-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="7e304-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="7e304-119">Spécifie le premier jour de la semaine.</span><span class="sxs-lookup"><span data-stu-id="7e304-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e304-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7e304-120">Parent elements</span></span>

|<span data-ttu-id="7e304-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7e304-121">**Element**</span></span>|<span data-ttu-id="7e304-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="7e304-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e304-123">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7e304-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7e304-124">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="7e304-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="7e304-125">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7e304-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="7e304-126">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="7e304-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e304-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7e304-127">Text value</span></span>

<span data-ttu-id="7e304-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e304-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e304-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e304-129">Remarks</span></span>

<span data-ttu-id="7e304-130">Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de [fin](end-ex15websvcsotherref.md) de l’élément périodique principal n’ont pas de date qui est égale à la première occurrence d’une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="7e304-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="7e304-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e304-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e304-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7e304-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e304-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7e304-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e304-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7e304-134">Schema Name</span></span>  <br/> |<span data-ttu-id="7e304-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7e304-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e304-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7e304-136">Validation File</span></span>  <br/> |<span data-ttu-id="7e304-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e304-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e304-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7e304-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e304-139">False</span><span class="sxs-lookup"><span data-stu-id="7e304-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e304-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e304-140">See also</span></span>



- [<span data-ttu-id="7e304-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7e304-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

