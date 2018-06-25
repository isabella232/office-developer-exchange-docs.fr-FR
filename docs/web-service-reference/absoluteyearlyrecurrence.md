---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: L’élément AbsoluteYearlyRecurrence représente une périodicité annuelle.
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756294"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="a2fe7-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a2fe7-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="a2fe7-104">L’élément **AbsoluteYearlyRecurrence** représente une périodicité annuelle.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="a2fe7-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="a2fe7-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2fe7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2fe7-106">Attributes and elements</span></span>

<span data-ttu-id="a2fe7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2fe7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2fe7-108">Attributes</span></span>

<span data-ttu-id="a2fe7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2fe7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2fe7-110">Child elements</span></span>

|<span data-ttu-id="a2fe7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2fe7-111">**Element**</span></span>|<span data-ttu-id="a2fe7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2fe7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fe7-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="a2fe7-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="a2fe7-114">Décrit le jour du mois à laquelle un élément périodique se produit.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="a2fe7-115">La plage de valeurs de cette propriété est 1 et 31.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="a2fe7-116">Si pour un mois donné, cette valeur est supérieure au nombre de jours dans le mois, le dernier jour du mois est supposé pour cette propriété.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="a2fe7-117">Mois (élément périodicité)</span><span class="sxs-lookup"><span data-stu-id="a2fe7-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="a2fe7-118">Décrit le mois dans lequel un élément périodique annuel se produit.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2fe7-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2fe7-119">Parent elements</span></span>

|<span data-ttu-id="a2fe7-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2fe7-120">**Element**</span></span>|<span data-ttu-id="a2fe7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2fe7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fe7-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a2fe7-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="a2fe7-123">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="a2fe7-124">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a2fe7-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="a2fe7-125">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2fe7-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2fe7-126">Remarks</span></span>

<span data-ttu-id="a2fe7-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a2fe7-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2fe7-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a2fe7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2fe7-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a2fe7-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2fe7-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a2fe7-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a2fe7-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a2fe7-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2fe7-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a2fe7-132">Validation File</span></span>  <br/> |<span data-ttu-id="a2fe7-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2fe7-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2fe7-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a2fe7-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="a2fe7-135">False</span><span class="sxs-lookup"><span data-stu-id="a2fe7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2fe7-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2fe7-136">See also</span></span>

- [<span data-ttu-id="a2fe7-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2fe7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

