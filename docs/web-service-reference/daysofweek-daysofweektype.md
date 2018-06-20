---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: L’élément DaysOfWeek indique les jours de la semaine qui sont utilisés dans l’élément périodicités.
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755829"
---
# <a name="daysofweek-daysofweektype"></a><span data-ttu-id="52761-103">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="52761-103">DaysOfWeek (DaysOfWeekType)</span></span>

<span data-ttu-id="52761-104">L’élément **DaysOfWeek** indique les jours de la semaine qui sont utilisés dans l’élément périodicités.</span><span class="sxs-lookup"><span data-stu-id="52761-104">The **DaysOfWeek** element describes days of the week that are used in item recurrence patterns.</span></span> 
  
```XML
<DaysOfWeek/>
```

<span data-ttu-id="52761-105">**DaysOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="52761-105">**DaysOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="52761-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="52761-106">Attributes and elements</span></span>

<span data-ttu-id="52761-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="52761-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52761-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="52761-108">Attributes</span></span>

<span data-ttu-id="52761-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="52761-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52761-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="52761-110">Child elements</span></span>

<span data-ttu-id="52761-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="52761-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52761-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="52761-112">Parent elements</span></span>

|<span data-ttu-id="52761-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="52761-113">**Element**</span></span>|<span data-ttu-id="52761-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="52761-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52761-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="52761-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="52761-116">Décrit une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="52761-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52761-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="52761-117">Text value</span></span>

<span data-ttu-id="52761-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="52761-118">A text value is required.</span></span> <span data-ttu-id="52761-119">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="52761-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="52761-120">Dimanche</span><span class="sxs-lookup"><span data-stu-id="52761-120">Sunday</span></span>    
- <span data-ttu-id="52761-121">Lundi</span><span class="sxs-lookup"><span data-stu-id="52761-121">Monday</span></span>    
- <span data-ttu-id="52761-122">Mardi</span><span class="sxs-lookup"><span data-stu-id="52761-122">Tuesday</span></span>    
- <span data-ttu-id="52761-123">Mercredi</span><span class="sxs-lookup"><span data-stu-id="52761-123">Wednesday</span></span>    
- <span data-ttu-id="52761-124">Jeudi</span><span class="sxs-lookup"><span data-stu-id="52761-124">Thursday</span></span>    
- <span data-ttu-id="52761-125">Vendredi</span><span class="sxs-lookup"><span data-stu-id="52761-125">Friday</span></span>    
- <span data-ttu-id="52761-126">Samedi</span><span class="sxs-lookup"><span data-stu-id="52761-126">Saturday</span></span>    
- <span data-ttu-id="52761-127">Day (cette valeur n’est pas valide pour une périodicité hebdomadaire)</span><span class="sxs-lookup"><span data-stu-id="52761-127">Day (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="52761-128">WeekDay (cette valeur n’est pas valide pour une périodicité hebdomadaire)</span><span class="sxs-lookup"><span data-stu-id="52761-128">Weekday (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="52761-129">WeekendDay (cette valeur n’est pas valide pour une périodicité hebdomadaire)</span><span class="sxs-lookup"><span data-stu-id="52761-129">WeekendDay (this value is not valid for a weekly recurrence pattern)</span></span>
    
<span data-ttu-id="52761-130">Une périodicité hebdomadaire peut contenir plusieurs valeurs.</span><span class="sxs-lookup"><span data-stu-id="52761-130">A weekly recurrence pattern can contain multiple values.</span></span> <span data-ttu-id="52761-131">Les valeurs sont séparées par un espace.</span><span class="sxs-lookup"><span data-stu-id="52761-131">Values are separated by a space character.</span></span> <span data-ttu-id="52761-132">Par exemple, pour une périodicité hebdomadaire mardi et le jeudi, la valeur de texte sera « Mardi jeudi ».</span><span class="sxs-lookup"><span data-stu-id="52761-132">For example, for a weekly recurrence on Tuesdays and Thursdays, the text value will be "Tuesday Thursday".</span></span>
  
## <a name="remarks"></a><span data-ttu-id="52761-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="52761-133">Remarks</span></span>

<span data-ttu-id="52761-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="52761-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52761-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="52761-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52761-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="52761-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52761-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="52761-137">Schema Name</span></span>  <br/> |<span data-ttu-id="52761-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="52761-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="52761-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="52761-139">Validation File</span></span>  <br/> |<span data-ttu-id="52761-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52761-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52761-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="52761-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="52761-142">False</span><span class="sxs-lookup"><span data-stu-id="52761-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52761-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="52761-143">See also</span></span>

- [<span data-ttu-id="52761-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="52761-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

