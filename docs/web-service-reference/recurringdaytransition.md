---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: L’élément RecurringDayTransition représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829012"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="6a2f4-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="6a2f4-103">RecurringDayTransition</span></span>

<span data-ttu-id="6a2f4-104">L’élément **RecurringDayTransition** représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="6a2f4-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="6a2f4-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a2f4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6a2f4-106">Attributes and elements</span></span>

<span data-ttu-id="6a2f4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a2f4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6a2f4-108">Attributes</span></span>

<span data-ttu-id="6a2f4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a2f4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6a2f4-110">Child elements</span></span>

|<span data-ttu-id="6a2f4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6a2f4-111">**Element**</span></span>|<span data-ttu-id="6a2f4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6a2f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a2f4-113">Pour</span><span class="sxs-lookup"><span data-stu-id="6a2f4-113">To</span></span>](to.md) <br/> |<span data-ttu-id="6a2f4-114">Spécifie la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="6a2f4-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2f4-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="6a2f4-116">Représente le décalage de la durée du temps universel coordonné (UTC) pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="6a2f4-117">Mois (Transition fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="6a2f4-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="6a2f4-118">Représente le mois dans laquelle se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="6a2f4-119">DayOfWeek (fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="6a2f4-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="6a2f4-120">Représente le jour de la semaine sur lequel se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="6a2f4-121">Occurrence (Transition fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="6a2f4-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="6a2f4-122">Représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a2f4-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6a2f4-123">Parent elements</span></span>

|<span data-ttu-id="6a2f4-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6a2f4-124">**Element**</span></span>|<span data-ttu-id="6a2f4-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="6a2f4-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a2f4-126">Transitions</span><span class="sxs-lookup"><span data-stu-id="6a2f4-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="6a2f4-127">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="6a2f4-128">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="6a2f4-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="6a2f4-129">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a2f4-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="6a2f4-130">Remarks</span></span>

<span data-ttu-id="6a2f4-131">Un exemple d’une transition de fuseau horaire qui peut être représenté par l’élément [RecurringDayTransition](recurringdaytransition.md) est une transition se produit le deuxième mardi du mois de février de chaque année.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="6a2f4-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6a2f4-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a2f4-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6a2f4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a2f4-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6a2f4-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a2f4-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6a2f4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="6a2f4-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6a2f4-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a2f4-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6a2f4-137">Validation File</span></span>  <br/> |<span data-ttu-id="6a2f4-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a2f4-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a2f4-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6a2f4-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a2f4-140">False</span><span class="sxs-lookup"><span data-stu-id="6a2f4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a2f4-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6a2f4-141">See also</span></span>



- [<span data-ttu-id="6a2f4-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6a2f4-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

