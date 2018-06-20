---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: L’élément AbsoluteMonthlyRecurrence représente une périodicité mensuelle.
ms.openlocfilehash: f4613fa71a9164c45b60a82f675959817cd4bdd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756299"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="294ef-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="294ef-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="294ef-104">L’élément **AbsoluteMonthlyRecurrence** représente une périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="294ef-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="294ef-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="294ef-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="294ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="294ef-106">Attributes and elements</span></span>

<span data-ttu-id="294ef-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="294ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="294ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="294ef-108">Attributes</span></span>

<span data-ttu-id="294ef-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="294ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="294ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="294ef-110">Child elements</span></span>

|<span data-ttu-id="294ef-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="294ef-111">**Element**</span></span>|<span data-ttu-id="294ef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="294ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="294ef-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="294ef-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="294ef-114">Décrit le jour du mois qui se produit un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="294ef-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="294ef-115">La plage de valeurs de cette propriété est 1 et 31.</span><span class="sxs-lookup"><span data-stu-id="294ef-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="294ef-116">Si pour un mois donné, cette valeur est supérieure au nombre de jours dans le mois, le dernier jour du mois est supposé pour cette propriété.</span><span class="sxs-lookup"><span data-stu-id="294ef-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="294ef-117">Intervalle</span><span class="sxs-lookup"><span data-stu-id="294ef-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="294ef-118">Définit l’intervalle entre deux éléments périodiques consécutives.</span><span class="sxs-lookup"><span data-stu-id="294ef-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="294ef-119">Par exemple, si l’élément de **l’intervalle** a la valeur 5, l’élément périodique se produit tous les mois 5.</span><span class="sxs-lookup"><span data-stu-id="294ef-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="294ef-120">La plage de valeurs valides est comprise entre 1 et 99.</span><span class="sxs-lookup"><span data-stu-id="294ef-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="294ef-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="294ef-121">Parent elements</span></span>

|<span data-ttu-id="294ef-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="294ef-122">**Element**</span></span>|<span data-ttu-id="294ef-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="294ef-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="294ef-124">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="294ef-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="294ef-125">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="294ef-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="294ef-126">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="294ef-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="294ef-127">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="294ef-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="294ef-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="294ef-128">Remarks</span></span>

<span data-ttu-id="294ef-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="294ef-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="294ef-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="294ef-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="294ef-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="294ef-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="294ef-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="294ef-132">Schema Name</span></span>  <br/> |<span data-ttu-id="294ef-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="294ef-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="294ef-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="294ef-134">Validation File</span></span>  <br/> |<span data-ttu-id="294ef-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="294ef-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="294ef-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="294ef-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="294ef-137">False</span><span class="sxs-lookup"><span data-stu-id="294ef-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="294ef-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="294ef-138">See also</span></span>

- [<span data-ttu-id="294ef-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="294ef-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

