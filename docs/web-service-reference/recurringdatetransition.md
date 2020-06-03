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
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461575"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="9f84f-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="9f84f-103">RecurringDateTransition</span></span>

<span data-ttu-id="9f84f-104">L’élément **RecurringDateTransition** représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.</span><span class="sxs-lookup"><span data-stu-id="9f84f-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="9f84f-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="9f84f-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f84f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f84f-106">Attributes and elements</span></span>

<span data-ttu-id="9f84f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f84f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f84f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f84f-108">Attributes</span></span>

<span data-ttu-id="9f84f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9f84f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f84f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f84f-110">Child elements</span></span>

|<span data-ttu-id="9f84f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f84f-111">**Element**</span></span>|<span data-ttu-id="9f84f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f84f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f84f-113">To</span><span class="sxs-lookup"><span data-stu-id="9f84f-113">To</span></span>](to.md) <br/> |<span data-ttu-id="9f84f-114">Spécifie le [point](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9f84f-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="9f84f-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f84f-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="9f84f-116">Représente le décalage de durée par rapport au temps universel coordonné (UTC) pour la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9f84f-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="9f84f-117">Mois (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="9f84f-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="9f84f-118">Représente le mois au cours duquel la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="9f84f-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="9f84f-119">Day</span><span class="sxs-lookup"><span data-stu-id="9f84f-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="9f84f-120">Représente le jour du mois où la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="9f84f-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f84f-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f84f-121">Parent elements</span></span>

|<span data-ttu-id="9f84f-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f84f-122">**Element**</span></span>|<span data-ttu-id="9f84f-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f84f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f84f-124">Transitions</span><span class="sxs-lookup"><span data-stu-id="9f84f-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="9f84f-125">Représente une collection de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9f84f-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="9f84f-126">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="9f84f-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="9f84f-127">Représente une collection de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="9f84f-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f84f-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f84f-128">Remarks</span></span>

<span data-ttu-id="9f84f-129">Un exemple de transition de fuseau horaire pouvant être représentée par l’élément [RecurringDateTransition](recurringdatetransition.md) est une transition qui a lieu le 15 mars de chaque année.</span><span class="sxs-lookup"><span data-stu-id="9f84f-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="9f84f-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9f84f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f84f-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f84f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f84f-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f84f-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f84f-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f84f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="9f84f-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9f84f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f84f-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f84f-135">Validation File</span></span>  <br/> |<span data-ttu-id="9f84f-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f84f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f84f-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f84f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f84f-138">False</span><span class="sxs-lookup"><span data-stu-id="9f84f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f84f-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f84f-139">See also</span></span>



- [<span data-ttu-id="9f84f-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f84f-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

