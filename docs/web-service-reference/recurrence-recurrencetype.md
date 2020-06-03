---
title: Récurrence (RecurrenceType)
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
description: L’élément Recurrence contient la périodicité des éléments de calendrier et des demandes de réunion.
ms.openlocfilehash: d00445c75fb35c3bb99eeed06e30cb1cf2883597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529888"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="4d6bb-103">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4d6bb-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="4d6bb-104">L’élément **Recurrence** contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

<span data-ttu-id="4d6bb-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="4d6bb-105">**RecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4d6bb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d6bb-106">Attributes and elements</span></span>

<span data-ttu-id="4d6bb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d6bb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d6bb-108">Attributes</span></span>

<span data-ttu-id="4d6bb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d6bb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d6bb-110">Child elements</span></span>

|<span data-ttu-id="4d6bb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d6bb-111">**Element**</span></span>|<span data-ttu-id="4d6bb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d6bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d6bb-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-114">Décrit une périodicité annuelle relative.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-116">Représente une périodicité annuelle.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-118">Décrit un modèle de périodicité mensuelle relative pour un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-120">Représente une périodicité mensuelle.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-122">Décrit la fréquence, en semaines, et les jours de récurrence d’un élément de calendrier ou d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="4d6bb-124">Décrit la fréquence, en jours, de récurrence d’une tâche ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="4d6bb-126">Décrit un modèle de récurrence qui n’a pas de date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="4d6bb-127">L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6bb-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="4d6bb-129">Décrit la date de début et la date de fin d’une périodicité d’élément.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="4d6bb-130">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6bb-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d6bb-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="4d6bb-132">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="4d6bb-133">L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="4d6bb-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d6bb-134">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d6bb-134">Parent elements</span></span>

|<span data-ttu-id="4d6bb-135">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d6bb-135">**Element**</span></span>|<span data-ttu-id="4d6bb-136">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d6bb-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d6bb-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4d6bb-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4d6bb-138">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4d6bb-139">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="4d6bb-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4d6bb-140">Représente une demande de réunion dans la Banque d’aide Exchange</span><span class="sxs-lookup"><span data-stu-id="4d6bb-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d6bb-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d6bb-141">Remarks</span></span>

<span data-ttu-id="4d6bb-142">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="4d6bb-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4d6bb-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d6bb-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d6bb-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d6bb-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d6bb-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d6bb-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d6bb-146">Schema name</span></span>  <br/> |<span data-ttu-id="4d6bb-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4d6bb-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d6bb-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d6bb-148">Validation file</span></span>  <br/> |<span data-ttu-id="4d6bb-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d6bb-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d6bb-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d6bb-150">Can be empty</span></span>  <br/> |<span data-ttu-id="4d6bb-151">False</span><span class="sxs-lookup"><span data-stu-id="4d6bb-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d6bb-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d6bb-152">See also</span></span>

- [<span data-ttu-id="4d6bb-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4d6bb-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

