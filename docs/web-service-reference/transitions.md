---
title: Transitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: L’élément transitions représente un tableau de transitions entre les fuseaux horaires.
ms.openlocfilehash: d48fb8872b2f7e052f733c32e5dd1c9b4d04d898
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467437"
---
# <a name="transitions"></a><span data-ttu-id="126e3-103">Transitions</span><span class="sxs-lookup"><span data-stu-id="126e3-103">Transitions</span></span>

<span data-ttu-id="126e3-104">L’élément **transitions** représente un tableau de transitions entre les fuseaux horaires.</span><span class="sxs-lookup"><span data-stu-id="126e3-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="126e3-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="126e3-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="126e3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="126e3-106">Attributes and elements</span></span>

<span data-ttu-id="126e3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="126e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="126e3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="126e3-108">Attributes</span></span>

|<span data-ttu-id="126e3-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="126e3-109">**Attribute**</span></span>|<span data-ttu-id="126e3-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="126e3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="126e3-111">ID</span><span class="sxs-lookup"><span data-stu-id="126e3-111">Id</span></span>  <br/> |<span data-ttu-id="126e3-112">Représente l’identificateur unique de la définition du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="126e3-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="126e3-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="126e3-113">Child elements</span></span>

|<span data-ttu-id="126e3-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="126e3-114">**Element**</span></span>|<span data-ttu-id="126e3-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="126e3-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="126e3-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="126e3-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="126e3-117">Représente une transition de fuseau horaire qui se produit à une date et à une heure spécifiques.</span><span class="sxs-lookup"><span data-stu-id="126e3-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="126e3-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="126e3-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="126e3-119">Représente une transition de fuseau horaire qui se produit chaque année.</span><span class="sxs-lookup"><span data-stu-id="126e3-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="126e3-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="126e3-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="126e3-121">Représente une transition de fuseau horaire qui se produit un jour de l’année donné.</span><span class="sxs-lookup"><span data-stu-id="126e3-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="126e3-122">Bascul</span><span class="sxs-lookup"><span data-stu-id="126e3-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="126e3-123">Représente une transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="126e3-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="126e3-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="126e3-124">Parent elements</span></span>

|<span data-ttu-id="126e3-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="126e3-125">**Element**</span></span>|<span data-ttu-id="126e3-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="126e3-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="126e3-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="126e3-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="126e3-128">Définit le fuseau horaire pour l’heure de début d’une [CalendarItem](calendaritem.md) ou d’un [propriété meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="126e3-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="126e3-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="126e3-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="126e3-130">Définit le fuseau horaire pour l’heure de fin d’une [CalendarItem](calendaritem.md) ou d’un [propriété meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="126e3-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="126e3-131">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="126e3-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="126e3-132">Définit un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="126e3-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="126e3-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="126e3-133">Text value</span></span>

<span data-ttu-id="126e3-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="126e3-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="126e3-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="126e3-135">Remarks</span></span>

<span data-ttu-id="126e3-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="126e3-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="126e3-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="126e3-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="126e3-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="126e3-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="126e3-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="126e3-139">Schema Name</span></span>  <br/> |<span data-ttu-id="126e3-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="126e3-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="126e3-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="126e3-141">Validation File</span></span>  <br/> |<span data-ttu-id="126e3-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="126e3-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="126e3-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="126e3-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="126e3-144">False</span><span class="sxs-lookup"><span data-stu-id="126e3-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="126e3-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="126e3-145">See also</span></span>



- [<span data-ttu-id="126e3-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="126e3-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

