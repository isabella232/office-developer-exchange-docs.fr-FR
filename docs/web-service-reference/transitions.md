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
description: L’élément Transitions représente un tableau des transitions de fuseau horaire.
ms.openlocfilehash: df7cacdef71c3fdfaa3ecadb486843ea30e6109d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838771"
---
# <a name="transitions"></a><span data-ttu-id="bca05-103">Transitions</span><span class="sxs-lookup"><span data-stu-id="bca05-103">Transitions</span></span>

<span data-ttu-id="bca05-104">L’élément **Transitions** représente un tableau des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bca05-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="bca05-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="bca05-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bca05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bca05-106">Attributes and elements</span></span>

<span data-ttu-id="bca05-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bca05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bca05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bca05-108">Attributes</span></span>

|<span data-ttu-id="bca05-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bca05-109">**Attribute**</span></span>|<span data-ttu-id="bca05-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bca05-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bca05-111">ID</span><span class="sxs-lookup"><span data-stu-id="bca05-111">Id</span></span>  <br/> |<span data-ttu-id="bca05-112">Identificateur unique de la définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bca05-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bca05-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bca05-113">Child elements</span></span>

|<span data-ttu-id="bca05-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bca05-114">**Element**</span></span>|<span data-ttu-id="bca05-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="bca05-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bca05-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="bca05-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="bca05-117">Représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.</span><span class="sxs-lookup"><span data-stu-id="bca05-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="bca05-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="bca05-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="bca05-119">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="bca05-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="bca05-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="bca05-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="bca05-121">Représente une transition de fuseau horaire qui se produit sur un jour spécifié de l’année.</span><span class="sxs-lookup"><span data-stu-id="bca05-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="bca05-122">Transition</span><span class="sxs-lookup"><span data-stu-id="bca05-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="bca05-123">Représente une transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bca05-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bca05-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bca05-124">Parent elements</span></span>

|<span data-ttu-id="bca05-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bca05-125">**Element**</span></span>|<span data-ttu-id="bca05-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="bca05-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bca05-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="bca05-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="bca05-128">Définit le fuseau horaire pour l’heure de début d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="bca05-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="bca05-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="bca05-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="bca05-130">Définit le fuseau horaire pour l’heure de fin d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="bca05-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="bca05-131">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="bca05-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="bca05-132">Définit un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bca05-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bca05-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bca05-133">Text value</span></span>

<span data-ttu-id="bca05-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bca05-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bca05-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="bca05-135">Remarks</span></span>

<span data-ttu-id="bca05-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bca05-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bca05-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bca05-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bca05-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bca05-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bca05-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bca05-139">Schema Name</span></span>  <br/> |<span data-ttu-id="bca05-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bca05-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="bca05-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bca05-141">Validation File</span></span>  <br/> |<span data-ttu-id="bca05-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bca05-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bca05-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bca05-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="bca05-144">False</span><span class="sxs-lookup"><span data-stu-id="bca05-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bca05-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bca05-145">See also</span></span>



- [<span data-ttu-id="bca05-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bca05-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

