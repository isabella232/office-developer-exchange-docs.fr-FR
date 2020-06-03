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
description: L’élément RelativeMonthlyRecurrence décrit un modèle de périodicité mensuelle relative.
ms.openlocfilehash: 90aa0e43684bfb09a3e13cf86ec96f680e80a714
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457507"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="7c824-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="7c824-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="7c824-104">L’élément **RelativeMonthlyRecurrence** décrit un modèle de périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="7c824-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="7c824-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="7c824-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c824-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7c824-106">Attributes and elements</span></span>

<span data-ttu-id="7c824-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7c824-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c824-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7c824-108">Attributes</span></span>

<span data-ttu-id="7c824-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7c824-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c824-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7c824-110">Child elements</span></span>

|<span data-ttu-id="7c824-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c824-111">**Element**</span></span>|<span data-ttu-id="7c824-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c824-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c824-113">Interval</span><span class="sxs-lookup"><span data-stu-id="7c824-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7c824-114">Définit l’intervalle entre deux éléments de motif périodique mensuel consécutifs.</span><span class="sxs-lookup"><span data-stu-id="7c824-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="7c824-115">La plage de cette valeur est comprise entre 1 et 99.</span><span class="sxs-lookup"><span data-stu-id="7c824-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="7c824-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="7c824-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="7c824-117">Décrit les jours de la semaine qui se trouvent dans le modèle de périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="7c824-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="7c824-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="7c824-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="7c824-119">Décrit la semaine utilisée dans un modèle de périodicité mensuelle relative.</span><span class="sxs-lookup"><span data-stu-id="7c824-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c824-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7c824-120">Parent elements</span></span>

|<span data-ttu-id="7c824-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c824-121">**Element**</span></span>|<span data-ttu-id="7c824-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c824-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c824-123">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7c824-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="7c824-124">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="7c824-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="7c824-125">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7c824-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7c824-126">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="7c824-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c824-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="7c824-127">Remarks</span></span>

<span data-ttu-id="7c824-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7c824-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c824-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7c824-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c824-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7c824-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c824-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7c824-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7c824-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7c824-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c824-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7c824-133">Validation File</span></span>  <br/> |<span data-ttu-id="7c824-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c824-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c824-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7c824-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c824-136">False</span><span class="sxs-lookup"><span data-stu-id="7c824-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c824-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7c824-137">See also</span></span>



- [<span data-ttu-id="7c824-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7c824-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

