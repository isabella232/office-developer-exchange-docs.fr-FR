---
title: Plutôt IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: L’élément plutôt IsEqualTo représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et donne la valeur true si elles sont égales.
ms.openlocfilehash: a7a7deed79c271be74bb2ff16dd86605d468721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828013"
---
# <a name="isequalto"></a><span data-ttu-id="68abd-103">Plutôt IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="68abd-103">IsEqualTo</span></span>

<span data-ttu-id="68abd-104">L’élément **plutôt IsEqualTo** représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et donne la valeur true si elles sont égales.</span><span class="sxs-lookup"><span data-stu-id="68abd-104">The **IsEqualTo** element represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span> 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

 <span data-ttu-id="68abd-105">**IsEqualToType**</span><span class="sxs-lookup"><span data-stu-id="68abd-105">**IsEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68abd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="68abd-106">Attributes and elements</span></span>

<span data-ttu-id="68abd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="68abd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68abd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="68abd-108">Attributes</span></span>

<span data-ttu-id="68abd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="68abd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68abd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="68abd-110">Child elements</span></span>

|<span data-ttu-id="68abd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="68abd-111">**Element**</span></span>|<span data-ttu-id="68abd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="68abd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68abd-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="68abd-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="68abd-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="68abd-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="68abd-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="68abd-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="68abd-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="68abd-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="68abd-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="68abd-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="68abd-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="68abd-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="68abd-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="68abd-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="68abd-120">Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="68abd-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68abd-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="68abd-121">Parent elements</span></span>

|<span data-ttu-id="68abd-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="68abd-122">**Element**</span></span>|<span data-ttu-id="68abd-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="68abd-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68abd-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="68abd-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="68abd-125">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="68abd-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="68abd-126">Pas</span><span class="sxs-lookup"><span data-stu-id="68abd-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="68abd-127">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="68abd-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="68abd-128">And</span><span class="sxs-lookup"><span data-stu-id="68abd-128">And</span></span>](and.md) <br/> |<span data-ttu-id="68abd-129">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="68abd-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="68abd-130">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="68abd-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="68abd-131">Or</span><span class="sxs-lookup"><span data-stu-id="68abd-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="68abd-132">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="68abd-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="68abd-133">[Ou](or.md) retourne true si un de ses enfants retourne true.</span><span class="sxs-lookup"><span data-stu-id="68abd-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="68abd-134">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="68abd-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68abd-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="68abd-135">Remarks</span></span>

<span data-ttu-id="68abd-136">Pour effectuer des comparaisons de chaînes, envisagez d’utiliser l’élément [contient](contains.md) , car elle fournit des options pour les paramètres correspondants, tels que la casse et les espaces.</span><span class="sxs-lookup"><span data-stu-id="68abd-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters, such as case and white space.</span></span> <span data-ttu-id="68abd-137">Utilisez l’élément [pas](not.md) en association avec l’élément [contient](contains.md) pour inverser le résultat.</span><span class="sxs-lookup"><span data-stu-id="68abd-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="68abd-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="68abd-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68abd-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="68abd-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68abd-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="68abd-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68abd-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="68abd-141">Schema Name</span></span>  <br/> |<span data-ttu-id="68abd-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="68abd-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="68abd-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="68abd-143">Validation File</span></span>  <br/> |<span data-ttu-id="68abd-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="68abd-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="68abd-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="68abd-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="68abd-146">False</span><span class="sxs-lookup"><span data-stu-id="68abd-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68abd-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="68abd-147">See also</span></span>



- [<span data-ttu-id="68abd-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68abd-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

