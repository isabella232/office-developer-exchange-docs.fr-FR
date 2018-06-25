---
title: RelativeMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: L’élément RelativeMonthlyRecurrence décrit une périodicité mensuelle relative.
ms.openlocfilehash: 9b695052c38e2693946837bf99f03baea093df08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829053"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="ec865-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ec865-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="ec865-104">L’élément **RelativeMonthlyRecurrence** décrit une périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="ec865-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="ec865-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="ec865-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec865-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec865-106">Attributes and elements</span></span>

<span data-ttu-id="ec865-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec865-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec865-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec865-108">Attributes</span></span>

<span data-ttu-id="ec865-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec865-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec865-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec865-110">Child elements</span></span>

|<span data-ttu-id="ec865-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec865-111">**Element**</span></span>|<span data-ttu-id="ec865-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec865-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec865-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="ec865-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="ec865-114">Définit l’intervalle entre deux éléments motif abonnement mensuel consécutives.</span><span class="sxs-lookup"><span data-stu-id="ec865-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="ec865-115">La plage pour que cette valeur est de 1 à 99.</span><span class="sxs-lookup"><span data-stu-id="ec865-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="ec865-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="ec865-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="ec865-117">Décrit les jours de la semaine dans la périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="ec865-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="ec865-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="ec865-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="ec865-119">Décrit la semaine est utilisée dans une périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="ec865-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec865-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec865-120">Parent elements</span></span>

|<span data-ttu-id="ec865-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec865-121">**Element**</span></span>|<span data-ttu-id="ec865-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec865-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec865-123">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ec865-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="ec865-124">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="ec865-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="ec865-125">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ec865-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ec865-126">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="ec865-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ec865-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec865-127">Remarks</span></span>

<span data-ttu-id="ec865-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec865-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec865-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec865-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec865-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec865-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec865-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec865-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ec865-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ec865-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec865-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec865-133">Validation File</span></span>  <br/> |<span data-ttu-id="ec865-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ec865-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec865-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec865-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec865-136">False</span><span class="sxs-lookup"><span data-stu-id="ec865-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec865-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec865-137">See also</span></span>



- [<span data-ttu-id="ec865-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec865-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

