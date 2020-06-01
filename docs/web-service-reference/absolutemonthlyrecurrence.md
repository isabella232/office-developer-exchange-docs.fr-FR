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
description: L’élément AbsoluteMonthlyRecurrence représente un modèle de périodicité mensuelle.
ms.openlocfilehash: 3176cd30a1cfe7b2310f960ce377ab7a277e795a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460434"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="67aba-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="67aba-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="67aba-104">L’élément **AbsoluteMonthlyRecurrence** représente un modèle de périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="67aba-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="67aba-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="67aba-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67aba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="67aba-106">Attributes and elements</span></span>

<span data-ttu-id="67aba-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="67aba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67aba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="67aba-108">Attributes</span></span>

<span data-ttu-id="67aba-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="67aba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67aba-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="67aba-110">Child elements</span></span>

|<span data-ttu-id="67aba-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67aba-111">**Element**</span></span>|<span data-ttu-id="67aba-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="67aba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67aba-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="67aba-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="67aba-114">Décrit le jour d’un mois pendant lequel un élément périodique se produit.</span><span class="sxs-lookup"><span data-stu-id="67aba-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="67aba-115">La plage de valeurs de cette propriété est comprise entre 1 et 31.</span><span class="sxs-lookup"><span data-stu-id="67aba-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="67aba-116">Si, pour un mois donné, cette valeur est supérieure au nombre de jours du mois, le dernier jour du mois est supposé pour cette propriété.</span><span class="sxs-lookup"><span data-stu-id="67aba-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="67aba-117">Interval</span><span class="sxs-lookup"><span data-stu-id="67aba-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="67aba-118">Définit l’intervalle entre deux éléments périodiques consécutifs.</span><span class="sxs-lookup"><span data-stu-id="67aba-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="67aba-119">Par exemple, si l’élément **Interval** a la valeur 5, l’élément périodique se produit tous les 5 mois.</span><span class="sxs-lookup"><span data-stu-id="67aba-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="67aba-120">La plage de valeurs valide est comprise entre 1 et 99.</span><span class="sxs-lookup"><span data-stu-id="67aba-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67aba-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="67aba-121">Parent elements</span></span>

|<span data-ttu-id="67aba-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67aba-122">**Element**</span></span>|<span data-ttu-id="67aba-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="67aba-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67aba-124">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="67aba-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="67aba-125">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="67aba-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="67aba-126">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="67aba-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="67aba-127">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="67aba-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="67aba-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="67aba-128">Remarks</span></span>

<span data-ttu-id="67aba-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="67aba-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67aba-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="67aba-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67aba-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="67aba-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67aba-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="67aba-132">Schema Name</span></span>  <br/> |<span data-ttu-id="67aba-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="67aba-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="67aba-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="67aba-134">Validation File</span></span>  <br/> |<span data-ttu-id="67aba-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67aba-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67aba-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="67aba-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="67aba-137">False</span><span class="sxs-lookup"><span data-stu-id="67aba-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67aba-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67aba-138">See also</span></span>

- [<span data-ttu-id="67aba-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="67aba-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

