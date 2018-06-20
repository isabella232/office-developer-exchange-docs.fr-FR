---
title: Périodicité (TaskRecurrenceType)
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
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: L’élément de périodicité contient des informations de périodicité pour les tâches répétitives.
ms.openlocfilehash: ae2bb35e89a0a50c7ca67cb0e580427150afb99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829006"
---
# <a name="recurrence-taskrecurrencetype"></a><span data-ttu-id="f9fe7-103">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f9fe7-103">Recurrence (TaskRecurrenceType)</span></span>

<span data-ttu-id="f9fe7-104">L’élément de **périodicité** contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-104">The **Recurrence** element contains recurrence information for recurring tasks.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="f9fe7-105">**TaskRecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="f9fe7-105">**TaskRecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9fe7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9fe7-106">Attributes and elements</span></span>

<span data-ttu-id="f9fe7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9fe7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9fe7-108">Attributes</span></span>

<span data-ttu-id="f9fe7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9fe7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9fe7-110">Child elements</span></span>

|<span data-ttu-id="f9fe7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9fe7-111">**Element**</span></span>|<span data-ttu-id="f9fe7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9fe7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fe7-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-114">Décrit une périodicité annuelle relative d’une tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-114">Describes a relative yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-116">Représente une périodicité annuelle pour une tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-116">Represents a yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-118">Décrit une périodicité mensuelle relative d’une tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-118">Describes a relative monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-120">Représente une périodicité mensuelle pour une tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-120">Represents a monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-122">Décrit la fréquence, en semaines et les jours où une tâche est périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-122">Describes the frequency, in weeks, and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="f9fe7-124">Décrit la fréquence, en jours, dans laquelle une tâche est périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-124">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-125">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="f9fe7-125">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="f9fe7-126">Décrit le nombre de jours après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-126">Describes how many days after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="f9fe7-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="f9fe7-128">Décrit le nombre de semaines après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-128">Describes how many weeks after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-129">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="f9fe7-129">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="f9fe7-130">Décrit le nombre de mois après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-130">Describes how many months after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-131">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="f9fe7-131">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="f9fe7-132">Indique combien d’années après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-132">Describes how many years after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-133">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-133">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="f9fe7-134">Décrit une périodicité qui n’a pas une date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-134">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="f9fe7-135">L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="f9fe7-135">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-136">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-136">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="f9fe7-137">Décrit la date de début et date de fin de périodicité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-137">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="f9fe7-138">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="f9fe7-138">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> <span data-ttu-id="f9fe7-139">[EndDateRecurrence](enddaterecurrence.md) ne peut pas être utilisé avec un motif de régénération.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-139">[EndDateRecurrence](enddaterecurrence.md) cannot be used together with a regeneration pattern.</span></span>  <br/> |
|[<span data-ttu-id="f9fe7-140">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9fe7-140">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="f9fe7-141">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-141">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="f9fe7-142">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="f9fe7-142">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9fe7-143">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9fe7-143">Parent elements</span></span>

|<span data-ttu-id="f9fe7-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9fe7-144">**Element**</span></span>|<span data-ttu-id="f9fe7-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9fe7-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fe7-146">Tâche</span><span class="sxs-lookup"><span data-stu-id="f9fe7-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="f9fe7-147">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-147">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9fe7-148">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9fe7-148">Remarks</span></span>

<span data-ttu-id="f9fe7-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f9fe7-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9fe7-150">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9fe7-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9fe7-151">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9fe7-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9fe7-152">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9fe7-152">Schema name</span></span>  <br/> |<span data-ttu-id="f9fe7-153">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f9fe7-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9fe7-154">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9fe7-154">Validation file</span></span>  <br/> |<span data-ttu-id="f9fe7-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9fe7-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9fe7-156">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9fe7-156">Can be empty</span></span>  <br/> |<span data-ttu-id="f9fe7-157">False</span><span class="sxs-lookup"><span data-stu-id="f9fe7-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9fe7-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9fe7-158">See also</span></span>



- [<span data-ttu-id="f9fe7-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f9fe7-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

