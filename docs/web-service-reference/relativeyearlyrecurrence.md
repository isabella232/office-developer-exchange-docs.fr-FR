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
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829057"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="ad873-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ad873-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="ad873-104">L’élément **RelativeYearlyRecurrence** décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="ad873-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="ad873-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="ad873-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad873-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad873-106">Attributes and elements</span></span>

<span data-ttu-id="ad873-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad873-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad873-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad873-108">Attributes</span></span>

<span data-ttu-id="ad873-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad873-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad873-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad873-110">Child elements</span></span>

|<span data-ttu-id="ad873-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad873-111">**Element**</span></span>|<span data-ttu-id="ad873-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad873-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad873-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="ad873-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="ad873-114">Décrit les jours de la semaine qui sont utilisés dans l’élément périodicités.</span><span class="sxs-lookup"><span data-stu-id="ad873-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="ad873-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="ad873-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="ad873-116">Décrit la semaine du mois est utilisée dans une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="ad873-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="ad873-117">Mois (élément périodicité)</span><span class="sxs-lookup"><span data-stu-id="ad873-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="ad873-118">Décrit le mois quand un élément périodique annuel se produit.</span><span class="sxs-lookup"><span data-stu-id="ad873-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad873-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad873-119">Parent elements</span></span>

|<span data-ttu-id="ad873-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad873-120">**Element**</span></span>|<span data-ttu-id="ad873-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad873-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad873-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ad873-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ad873-123">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="ad873-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="ad873-124">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ad873-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="ad873-125">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="ad873-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="ad873-126">Standard</span><span class="sxs-lookup"><span data-stu-id="ad873-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="ad873-127">Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="ad873-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="ad873-128">Heure d’été</span><span class="sxs-lookup"><span data-stu-id="ad873-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="ad873-129">Représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.</span><span class="sxs-lookup"><span data-stu-id="ad873-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad873-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad873-130">Remarks</span></span>

<span data-ttu-id="ad873-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ad873-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad873-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad873-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad873-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad873-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad873-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad873-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ad873-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ad873-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad873-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad873-136">Validation File</span></span>  <br/> |<span data-ttu-id="ad873-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad873-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad873-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad873-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad873-139">False</span><span class="sxs-lookup"><span data-stu-id="ad873-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad873-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad873-140">See also</span></span>



- [<span data-ttu-id="ad873-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad873-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

