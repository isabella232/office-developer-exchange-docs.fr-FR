---
title: Périodicité (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: L’élément de périodicité contient la périodicité pour les éléments de calendrier et les demandes de réunion.
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829004"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="c5ea1-103">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="c5ea1-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="c5ea1-104">L’élément de **périodicité** contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="c5ea1-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="c5ea1-105">**RecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5ea1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c5ea1-106">Attributes and elements</span></span>

<span data-ttu-id="c5ea1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5ea1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c5ea1-108">Attributes</span></span>

<span data-ttu-id="c5ea1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5ea1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c5ea1-110">Child elements</span></span>

|<span data-ttu-id="c5ea1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5ea1-111">**Element**</span></span>|<span data-ttu-id="c5ea1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5ea1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5ea1-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-114">Décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-116">Représente une périodicité annuelle.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-118">Décrit une périodicité mensuelle relative d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-120">Représente une périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-122">Décrit la fréquence, en semaines, ainsi que les jours un élément de calendrier ou une tâche est périodique.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="c5ea1-124">Décrit la fréquence, en jours, dans laquelle un élément de calendrier ou une tâche est périodique.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="c5ea1-126">Décrit une périodicité qui n’a pas une date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="c5ea1-127">L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="c5ea1-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="c5ea1-129">Décrit la date de début et date de fin de périodicité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="c5ea1-130">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="c5ea1-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5ea1-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="c5ea1-132">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="c5ea1-133">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="c5ea1-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5ea1-134">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c5ea1-134">Parent elements</span></span>

|<span data-ttu-id="c5ea1-135">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5ea1-135">**Element**</span></span>|<span data-ttu-id="c5ea1-136">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5ea1-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5ea1-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c5ea1-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c5ea1-138">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c5ea1-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c5ea1-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c5ea1-140">Représente une demande de réunion dans la banque d’informations Exchange</span><span class="sxs-lookup"><span data-stu-id="c5ea1-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5ea1-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="c5ea1-141">Remarks</span></span>

<span data-ttu-id="c5ea1-142">Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="c5ea1-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c5ea1-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5ea1-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c5ea1-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5ea1-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c5ea1-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5ea1-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c5ea1-146">Schema name</span></span>  <br/> |<span data-ttu-id="c5ea1-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c5ea1-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5ea1-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c5ea1-148">Validation file</span></span>  <br/> |<span data-ttu-id="c5ea1-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c5ea1-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5ea1-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c5ea1-150">Can be empty</span></span>  <br/> |<span data-ttu-id="c5ea1-151">False</span><span class="sxs-lookup"><span data-stu-id="c5ea1-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5ea1-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5ea1-152">See also</span></span>



- [<span data-ttu-id="c5ea1-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c5ea1-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
