---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: L’élément RelativeYearlyRecurrence décrit une périodicité annuelle relative.
ms.openlocfilehash: 2abe09ddfe52c24211ef5d0a392ddecaf15bf7bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456727"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="d0e50-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="d0e50-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="d0e50-104">L’élément **RelativeYearlyRecurrence** décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="d0e50-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="d0e50-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="d0e50-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0e50-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d0e50-106">Attributes and elements</span></span>

<span data-ttu-id="d0e50-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d0e50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0e50-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d0e50-108">Attributes</span></span>

<span data-ttu-id="d0e50-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d0e50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0e50-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d0e50-110">Child elements</span></span>

|<span data-ttu-id="d0e50-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0e50-111">**Element**</span></span>|<span data-ttu-id="d0e50-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0e50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0e50-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="d0e50-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="d0e50-114">Décrit les jours de la semaine utilisés dans les périodicités d’élément.</span><span class="sxs-lookup"><span data-stu-id="d0e50-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="d0e50-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="d0e50-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="d0e50-116">Indique quelle semaine d’un mois est utilisée dans une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="d0e50-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="d0e50-117">Month (périodicité de l’élément)</span><span class="sxs-lookup"><span data-stu-id="d0e50-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="d0e50-118">Décrit le mois auquel un élément périodique périodique se produit.</span><span class="sxs-lookup"><span data-stu-id="d0e50-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0e50-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d0e50-119">Parent elements</span></span>

|<span data-ttu-id="d0e50-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0e50-120">**Element**</span></span>|<span data-ttu-id="d0e50-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0e50-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0e50-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d0e50-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d0e50-123">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="d0e50-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="d0e50-124">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d0e50-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d0e50-125">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="d0e50-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="d0e50-126">Standard</span><span class="sxs-lookup"><span data-stu-id="d0e50-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="d0e50-127">Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="d0e50-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="d0e50-128">Auxquelles</span><span class="sxs-lookup"><span data-stu-id="d0e50-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="d0e50-129">Représente la date et l’heure auxquelles l’heure passe de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="d0e50-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d0e50-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="d0e50-130">Remarks</span></span>

<span data-ttu-id="d0e50-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d0e50-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0e50-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d0e50-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0e50-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d0e50-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0e50-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d0e50-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d0e50-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d0e50-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0e50-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d0e50-136">Validation File</span></span>  <br/> |<span data-ttu-id="d0e50-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0e50-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0e50-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d0e50-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0e50-139">False</span><span class="sxs-lookup"><span data-stu-id="d0e50-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0e50-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0e50-140">See also</span></span>



- [<span data-ttu-id="d0e50-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d0e50-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

