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
description: L’élément RecurringDayTransition représente une transition de fuseau horaire qui se produit chaque année le même jour.
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468466"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="741e6-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="741e6-103">RecurringDayTransition</span></span>

<span data-ttu-id="741e6-104">L’élément **RecurringDayTransition** représente une transition de fuseau horaire qui se produit chaque année le même jour.</span><span class="sxs-lookup"><span data-stu-id="741e6-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="741e6-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="741e6-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="741e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="741e6-106">Attributes and elements</span></span>

<span data-ttu-id="741e6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="741e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="741e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="741e6-108">Attributes</span></span>

<span data-ttu-id="741e6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="741e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="741e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="741e6-110">Child elements</span></span>

|<span data-ttu-id="741e6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="741e6-111">**Element**</span></span>|<span data-ttu-id="741e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="741e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="741e6-113">To</span><span class="sxs-lookup"><span data-stu-id="741e6-113">To</span></span>](to.md) <br/> |<span data-ttu-id="741e6-114">Spécifie le [point](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="741e6-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="741e6-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="741e6-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="741e6-116">Représente le décalage de durée par rapport au temps universel coordonné (UTC) pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="741e6-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="741e6-117">Mois (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="741e6-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="741e6-118">Représente le mois au cours duquel la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="741e6-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="741e6-119">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="741e6-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="741e6-120">Représente le jour de la semaine où la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="741e6-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="741e6-121">Occurrence (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="741e6-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="741e6-122">Représente l’occurrence du jour de la semaine du mois où la transition de fuseau horaire se produit.</span><span class="sxs-lookup"><span data-stu-id="741e6-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="741e6-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="741e6-123">Parent elements</span></span>

|<span data-ttu-id="741e6-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="741e6-124">**Element**</span></span>|<span data-ttu-id="741e6-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="741e6-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="741e6-126">Transitions</span><span class="sxs-lookup"><span data-stu-id="741e6-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="741e6-127">Représente une collection de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="741e6-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="741e6-128">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="741e6-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="741e6-129">Représente une collection de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="741e6-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="741e6-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="741e6-130">Remarks</span></span>

<span data-ttu-id="741e6-131">Un exemple de transition de fuseau horaire qui pourrait être représentée par l’élément [RecurringDayTransition](recurringdaytransition.md) est une transition qui a lieu le deuxième mardi de février chaque année.</span><span class="sxs-lookup"><span data-stu-id="741e6-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="741e6-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="741e6-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="741e6-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="741e6-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="741e6-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="741e6-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="741e6-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="741e6-135">Schema Name</span></span>  <br/> |<span data-ttu-id="741e6-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="741e6-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="741e6-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="741e6-137">Validation File</span></span>  <br/> |<span data-ttu-id="741e6-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="741e6-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="741e6-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="741e6-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="741e6-140">False</span><span class="sxs-lookup"><span data-stu-id="741e6-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="741e6-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="741e6-141">See also</span></span>



- [<span data-ttu-id="741e6-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="741e6-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

