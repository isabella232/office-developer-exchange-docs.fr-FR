---
title: Occurrence (transition de fuseau horaire)
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
description: L’élément occurrence représente l’occurrence du jour de la semaine du mois pendant lequel la transition de fuseau horaire a lieu.
ms.openlocfilehash: 846f6b22f43bcda07b9408d768d0845a5acfe668
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467976"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="be6d8-103">Occurrence (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="be6d8-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="be6d8-104">L’élément **occurrence** représente l’occurrence du jour de la semaine du mois pendant lequel la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="be6d8-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="be6d8-105">**int**</span><span class="sxs-lookup"><span data-stu-id="be6d8-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="be6d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="be6d8-106">Attributes and elements</span></span>

<span data-ttu-id="be6d8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="be6d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be6d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="be6d8-108">Attributes</span></span>

<span data-ttu-id="be6d8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="be6d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be6d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="be6d8-110">Child elements</span></span>

<span data-ttu-id="be6d8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="be6d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be6d8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="be6d8-112">Parent elements</span></span>

|<span data-ttu-id="be6d8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be6d8-113">**Element**</span></span>|<span data-ttu-id="be6d8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="be6d8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be6d8-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="be6d8-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="be6d8-116">Représente une transition de fuseau horaire qui se produit chaque année.</span><span class="sxs-lookup"><span data-stu-id="be6d8-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be6d8-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="be6d8-117">Text value</span></span>

<span data-ttu-id="be6d8-118">La valeur de texte est un entier qui représente l’occurrence du jour de la semaine du mois où la transition de fuseau horaire a lieu.</span><span class="sxs-lookup"><span data-stu-id="be6d8-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="be6d8-119">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="be6d8-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="be6d8-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="be6d8-120">**Value**</span></span>|<span data-ttu-id="be6d8-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="be6d8-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be6d8-122">0,1</span><span class="sxs-lookup"><span data-stu-id="be6d8-122">1</span></span>  <br/> |<span data-ttu-id="be6d8-123">Première occurrence du jour de la semaine spécifié à partir du début du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-124">n°2</span><span class="sxs-lookup"><span data-stu-id="be6d8-124">2</span></span>  <br/> |<span data-ttu-id="be6d8-125">Deuxième occurrence du jour de la semaine spécifié à partir du début du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-126">3</span><span class="sxs-lookup"><span data-stu-id="be6d8-126">3</span></span>  <br/> |<span data-ttu-id="be6d8-127">Troisième occurrence du jour de la semaine spécifié à partir du début du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-128">4 </span><span class="sxs-lookup"><span data-stu-id="be6d8-128">4</span></span>  <br/> |<span data-ttu-id="be6d8-129">Quatrième occurrence du jour de la semaine spécifié à partir du début du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-130">-1</span><span class="sxs-lookup"><span data-stu-id="be6d8-130">-1</span></span>  <br/> |<span data-ttu-id="be6d8-131">Première occurrence du jour de la semaine spécifié à partir de la fin du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-132">-2</span><span class="sxs-lookup"><span data-stu-id="be6d8-132">-2</span></span>  <br/> |<span data-ttu-id="be6d8-133">Deuxième occurrence du jour de la semaine spécifié à partir de la fin du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-134">-3</span><span class="sxs-lookup"><span data-stu-id="be6d8-134">-3</span></span>  <br/> |<span data-ttu-id="be6d8-135">Troisième occurrence du jour de la semaine spécifié à partir de la fin du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="be6d8-136">-4</span><span class="sxs-lookup"><span data-stu-id="be6d8-136">-4</span></span>  <br/> |<span data-ttu-id="be6d8-137">Quatrième occurrence du jour de la semaine spécifié à partir de la fin du mois.</span><span class="sxs-lookup"><span data-stu-id="be6d8-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="be6d8-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="be6d8-138">Remarks</span></span>

<span data-ttu-id="be6d8-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="be6d8-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be6d8-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="be6d8-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be6d8-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="be6d8-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be6d8-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="be6d8-142">Schema Name</span></span>  <br/> |<span data-ttu-id="be6d8-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="be6d8-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="be6d8-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="be6d8-144">Validation File</span></span>  <br/> |<span data-ttu-id="be6d8-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="be6d8-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be6d8-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="be6d8-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="be6d8-147">False</span><span class="sxs-lookup"><span data-stu-id="be6d8-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be6d8-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be6d8-148">See also</span></span>

- [<span data-ttu-id="be6d8-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="be6d8-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

