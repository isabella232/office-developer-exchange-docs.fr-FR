---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: L’élément RecurringDateTransition représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.
ms.openlocfilehash: 7cd8f3452a744e0c9a98fd3698dffb9ed8721a6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829014"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="e49a6-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="e49a6-103">RecurringDateTransition</span></span>

<span data-ttu-id="e49a6-104">L’élément **RecurringDateTransition** représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.</span><span class="sxs-lookup"><span data-stu-id="e49a6-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="e49a6-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="e49a6-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e49a6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e49a6-106">Attributes and elements</span></span>

<span data-ttu-id="e49a6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e49a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e49a6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e49a6-108">Attributes</span></span>

<span data-ttu-id="e49a6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e49a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e49a6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e49a6-110">Child elements</span></span>

|<span data-ttu-id="e49a6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e49a6-111">**Element**</span></span>|<span data-ttu-id="e49a6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e49a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e49a6-113">Pour</span><span class="sxs-lookup"><span data-stu-id="e49a6-113">To</span></span>](to.md) <br/> |<span data-ttu-id="e49a6-114">Spécifie la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="e49a6-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49a6-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="e49a6-116">Représente le décalage de la durée du temps universel coordonné (UTC) pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="e49a6-117">Mois (Transition fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="e49a6-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="e49a6-118">Représente le mois dans laquelle se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="e49a6-119">Jour</span><span class="sxs-lookup"><span data-stu-id="e49a6-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="e49a6-120">Représente le jour du mois sur lequel se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e49a6-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e49a6-121">Parent elements</span></span>

|<span data-ttu-id="e49a6-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e49a6-122">**Element**</span></span>|<span data-ttu-id="e49a6-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="e49a6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e49a6-124">Transitions</span><span class="sxs-lookup"><span data-stu-id="e49a6-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e49a6-125">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e49a6-126">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="e49a6-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="e49a6-127">Représente une collection des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="e49a6-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e49a6-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="e49a6-128">Remarks</span></span>

<span data-ttu-id="e49a6-129">Un exemple d’une transition de fuseau horaire qui peut être représenté par l’élément [RecurringDateTransition](recurringdatetransition.md) est une transition se produit le 15 mars de chaque année.</span><span class="sxs-lookup"><span data-stu-id="e49a6-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="e49a6-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="e49a6-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e49a6-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e49a6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e49a6-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e49a6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e49a6-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e49a6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e49a6-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e49a6-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e49a6-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e49a6-135">Validation File</span></span>  <br/> |<span data-ttu-id="e49a6-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e49a6-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e49a6-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e49a6-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e49a6-138">False</span><span class="sxs-lookup"><span data-stu-id="e49a6-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e49a6-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e49a6-139">See also</span></span>



- [<span data-ttu-id="e49a6-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e49a6-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

