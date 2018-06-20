---
title: Action
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: L’élément To spécifie la cible de la transition de fuseau horaire. La cible est une période de fuseau horaire ou un groupe des transitions de fuseau horaire.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838730"
---
# <a name="to"></a><span data-ttu-id="7da21-104">Action</span><span class="sxs-lookup"><span data-stu-id="7da21-104">To</span></span>

<span data-ttu-id="7da21-105">L’élément **To** spécifie la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="7da21-106">La cible est une période de fuseau horaire ou un groupe des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="7da21-107">**TransitionTargetType**</span><span class="sxs-lookup"><span data-stu-id="7da21-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7da21-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7da21-108">Attributes and elements</span></span>

<span data-ttu-id="7da21-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7da21-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da21-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7da21-110">Attributes</span></span>

|<span data-ttu-id="7da21-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7da21-111">**Attribute**</span></span>|<span data-ttu-id="7da21-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da21-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7da21-113">Type</span><span class="sxs-lookup"><span data-stu-id="7da21-113">Kind</span></span>  <br/> |<span data-ttu-id="7da21-114">Indique si la cible de transition de fuseau horaire est une période de fuseau horaire ou d’un groupe de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="7da21-115">Valeurs d’attribut de type</span><span class="sxs-lookup"><span data-stu-id="7da21-115">Kind attribute values</span></span>

|<span data-ttu-id="7da21-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7da21-116">**Value**</span></span>|<span data-ttu-id="7da21-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da21-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7da21-118">Point</span><span class="sxs-lookup"><span data-stu-id="7da21-118">Period</span></span>  <br/> |<span data-ttu-id="7da21-119">Spécifie que la cible de transition de fuseau horaire est une période de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="7da21-120">Groupe</span><span class="sxs-lookup"><span data-stu-id="7da21-120">Group</span></span>  <br/> |<span data-ttu-id="7da21-121">Spécifie que la cible de transition de fuseau horaire est un groupe de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7da21-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7da21-122">Child elements</span></span>

<span data-ttu-id="7da21-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da21-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7da21-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7da21-124">Parent elements</span></span>

|<span data-ttu-id="7da21-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7da21-125">**Element**</span></span>|<span data-ttu-id="7da21-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da21-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da21-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="7da21-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="7da21-128">Représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.</span><span class="sxs-lookup"><span data-stu-id="7da21-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="7da21-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="7da21-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="7da21-130">Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.</span><span class="sxs-lookup"><span data-stu-id="7da21-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="7da21-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="7da21-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="7da21-132">Représente une transition de fuseau horaire qui se produit sur un jour spécifié de l’année.</span><span class="sxs-lookup"><span data-stu-id="7da21-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="7da21-133">Transition</span><span class="sxs-lookup"><span data-stu-id="7da21-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="7da21-134">Représente une transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7da21-135">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7da21-135">Text value</span></span>

<span data-ttu-id="7da21-136">La valeur de texte est une chaîne qui spécifie l’identificateur unique de la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="7da21-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7da21-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="7da21-137">Remarks</span></span>

<span data-ttu-id="7da21-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="7da21-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7da21-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7da21-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7da21-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7da21-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7da21-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7da21-141">Schema Name</span></span>  <br/> |<span data-ttu-id="7da21-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7da21-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="7da21-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7da21-143">Validation File</span></span>  <br/> |<span data-ttu-id="7da21-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7da21-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7da21-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7da21-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="7da21-146">False</span><span class="sxs-lookup"><span data-stu-id="7da21-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7da21-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7da21-147">See also</span></span>



- [<span data-ttu-id="7da21-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7da21-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

