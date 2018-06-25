---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: L’élément contient représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755584"
---
# <a name="contains"></a><span data-ttu-id="8fd01-103">Contains</span><span class="sxs-lookup"><span data-stu-id="8fd01-103">Contains</span></span>

<span data-ttu-id="8fd01-104">L’élément **contient** représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.</span><span class="sxs-lookup"><span data-stu-id="8fd01-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 <span data-ttu-id="8fd01-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="8fd01-105">**ContainsExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fd01-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8fd01-106">Attributes and elements</span></span>

<span data-ttu-id="8fd01-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8fd01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fd01-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8fd01-108">Attributes</span></span>

|<span data-ttu-id="8fd01-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8fd01-109">**Attribute**</span></span>|<span data-ttu-id="8fd01-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fd01-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8fd01-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="8fd01-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="8fd01-112">Identifie les limites d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="8fd01-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="8fd01-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="8fd01-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="8fd01-114">Détermine si la recherche ignore les cas et les espaces.</span><span class="sxs-lookup"><span data-stu-id="8fd01-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="8fd01-115">Valeurs des attributs ContainmentMode</span><span class="sxs-lookup"><span data-stu-id="8fd01-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="8fd01-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="8fd01-116">**Value**</span></span>|<span data-ttu-id="8fd01-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fd01-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8fd01-118">FullString</span><span class="sxs-lookup"><span data-stu-id="8fd01-118">FullString</span></span>  <br/> |<span data-ttu-id="8fd01-119">La comparaison est comprise entre la chaîne complète et la constante.</span><span class="sxs-lookup"><span data-stu-id="8fd01-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="8fd01-120">La valeur de la propriété et la constante fournie sont exactement les mêmes.</span><span class="sxs-lookup"><span data-stu-id="8fd01-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="8fd01-121">Le préfixe</span><span class="sxs-lookup"><span data-stu-id="8fd01-121">Prefixed</span></span>  <br/> |<span data-ttu-id="8fd01-122">La comparaison est comprise entre le préfixe de la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="8fd01-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="8fd01-123">Sous-chaîne</span><span class="sxs-lookup"><span data-stu-id="8fd01-123">Substring</span></span>  <br/> |<span data-ttu-id="8fd01-124">La comparaison est comprise entre une sous-chaîne de la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="8fd01-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="8fd01-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="8fd01-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="8fd01-126">La comparaison est comprise entre un préfixe sur les mots individuels dans la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="8fd01-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="8fd01-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="8fd01-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="8fd01-128">La comparaison est comprise entre une expression exacte dans la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="8fd01-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="8fd01-129">Valeurs des attributs ContainmentComparison</span><span class="sxs-lookup"><span data-stu-id="8fd01-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="8fd01-130">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="8fd01-130">**Value**</span></span>|<span data-ttu-id="8fd01-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fd01-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8fd01-132">Exact</span><span class="sxs-lookup"><span data-stu-id="8fd01-132">Exact</span></span>  <br/> |<span data-ttu-id="8fd01-133">La comparaison doit être exacte.</span><span class="sxs-lookup"><span data-stu-id="8fd01-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="8fd01-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="8fd01-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="8fd01-135">La comparaison ignore la casse.</span><span class="sxs-lookup"><span data-stu-id="8fd01-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="8fd01-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="8fd01-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="8fd01-137">La comparaison ignore les caractères sans espace.</span><span class="sxs-lookup"><span data-stu-id="8fd01-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="8fd01-138">Espacé</span><span class="sxs-lookup"><span data-stu-id="8fd01-138">Loose</span></span>  <br/> |<span data-ttu-id="8fd01-139">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="8fd01-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="8fd01-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="8fd01-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="8fd01-141">La comparaison ignore la casse et non pas d’espacement des caractères.</span><span class="sxs-lookup"><span data-stu-id="8fd01-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="8fd01-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="8fd01-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="8fd01-143">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="8fd01-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="8fd01-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="8fd01-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="8fd01-145">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="8fd01-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="8fd01-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="8fd01-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="8fd01-147">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="8fd01-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8fd01-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8fd01-148">Child elements</span></span>

|<span data-ttu-id="8fd01-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fd01-149">**Element**</span></span>|<span data-ttu-id="8fd01-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fd01-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fd01-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="8fd01-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="8fd01-152">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="8fd01-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="8fd01-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="8fd01-154">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="8fd01-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="8fd01-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="8fd01-156">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="8fd01-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-157">Constante</span><span class="sxs-lookup"><span data-stu-id="8fd01-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="8fd01-158">Identifie une valeur de constante dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="8fd01-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8fd01-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8fd01-159">Parent elements</span></span>

|<span data-ttu-id="8fd01-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fd01-160">**Element**</span></span>|<span data-ttu-id="8fd01-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fd01-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fd01-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="8fd01-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="8fd01-163">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="8fd01-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-164">Pas</span><span class="sxs-lookup"><span data-stu-id="8fd01-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="8fd01-165">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="8fd01-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-166">And</span><span class="sxs-lookup"><span data-stu-id="8fd01-166">And</span></span>](and.md) <br/> |<span data-ttu-id="8fd01-167">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="8fd01-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="8fd01-168">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="8fd01-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="8fd01-169">Or</span><span class="sxs-lookup"><span data-stu-id="8fd01-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="8fd01-170">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="8fd01-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="8fd01-171">L’élément [ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="8fd01-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8fd01-172">Remarques</span><span class="sxs-lookup"><span data-stu-id="8fd01-172">Remarks</span></span>

<span data-ttu-id="8fd01-173">Les attributs sont utilisés pour déterminer la façon dont les éléments sont mis en correspondance.</span><span class="sxs-lookup"><span data-stu-id="8fd01-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="8fd01-174">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8fd01-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fd01-175">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8fd01-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fd01-176">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8fd01-176">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fd01-177">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8fd01-177">Schema Name</span></span>  <br/> |<span data-ttu-id="8fd01-178">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8fd01-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fd01-179">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8fd01-179">Validation File</span></span>  <br/> |<span data-ttu-id="8fd01-180">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fd01-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fd01-181">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8fd01-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fd01-182">False</span><span class="sxs-lookup"><span data-stu-id="8fd01-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fd01-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8fd01-183">See also</span></span>



- [<span data-ttu-id="8fd01-184">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8fd01-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

