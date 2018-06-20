---
title: Occurrence (Transition fuseau horaire)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: L’élément Occurrence représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828636"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="2bcdd-103">Occurrence (Transition fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="2bcdd-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="2bcdd-104">L’élément **Occurrence** représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="2bcdd-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2bcdd-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2bcdd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2bcdd-106">Attributes and elements</span></span>

<span data-ttu-id="2bcdd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bcdd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2bcdd-108">Attributes</span></span>

<span data-ttu-id="2bcdd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bcdd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2bcdd-110">Child elements</span></span>

<span data-ttu-id="2bcdd-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2bcdd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2bcdd-112">Parent elements</span></span>

|<span data-ttu-id="2bcdd-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2bcdd-113">**Element**</span></span>|<span data-ttu-id="2bcdd-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bcdd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bcdd-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="2bcdd-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="2bcdd-116">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2bcdd-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2bcdd-117">Text value</span></span>

<span data-ttu-id="2bcdd-118">La valeur de texte est un entier qui représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="2bcdd-119">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="2bcdd-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2bcdd-120">**Value**</span></span>|<span data-ttu-id="2bcdd-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bcdd-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2bcdd-122">1</span><span class="sxs-lookup"><span data-stu-id="2bcdd-122">1</span></span>  <br/> |<span data-ttu-id="2bcdd-123">La première occurrence du jour de la semaine à partir du début du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-124">2</span><span class="sxs-lookup"><span data-stu-id="2bcdd-124">2</span></span>  <br/> |<span data-ttu-id="2bcdd-125">La deuxième occurrence du jour de la semaine à partir du début du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-126">3</span><span class="sxs-lookup"><span data-stu-id="2bcdd-126">3</span></span>  <br/> |<span data-ttu-id="2bcdd-127">La troisième occurrence du jour de la semaine à partir du début du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-128">4</span><span class="sxs-lookup"><span data-stu-id="2bcdd-128">4</span></span>  <br/> |<span data-ttu-id="2bcdd-129">La quatrième occurrence du jour de la semaine à partir du début du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-130">-1</span><span class="sxs-lookup"><span data-stu-id="2bcdd-130">-1</span></span>  <br/> |<span data-ttu-id="2bcdd-131">La première occurrence du jour de semaine à partir de la fin du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-132">-2</span><span class="sxs-lookup"><span data-stu-id="2bcdd-132">-2</span></span>  <br/> |<span data-ttu-id="2bcdd-133">La deuxième occurrence du jour de semaine à partir de la fin du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-134">-3</span><span class="sxs-lookup"><span data-stu-id="2bcdd-134">-3</span></span>  <br/> |<span data-ttu-id="2bcdd-135">La troisième occurrence du jour de semaine à partir de la fin du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="2bcdd-136">-4</span><span class="sxs-lookup"><span data-stu-id="2bcdd-136">-4</span></span>  <br/> |<span data-ttu-id="2bcdd-137">La quatrième occurrence du jour de semaine à partir de la fin du mois spécifié.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2bcdd-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="2bcdd-138">Remarks</span></span>

<span data-ttu-id="2bcdd-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="2bcdd-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bcdd-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2bcdd-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bcdd-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2bcdd-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2bcdd-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2bcdd-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2bcdd-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2bcdd-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="2bcdd-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2bcdd-144">Validation File</span></span>  <br/> |<span data-ttu-id="2bcdd-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2bcdd-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2bcdd-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2bcdd-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bcdd-147">False</span><span class="sxs-lookup"><span data-stu-id="2bcdd-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bcdd-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2bcdd-148">See also</span></span>

- [<span data-ttu-id="2bcdd-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2bcdd-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

