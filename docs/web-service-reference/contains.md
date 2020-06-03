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
description: L’élément Contains représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527116"
---
# <a name="contains"></a><span data-ttu-id="fe419-103">Contains</span><span class="sxs-lookup"><span data-stu-id="fe419-103">Contains</span></span>

<span data-ttu-id="fe419-104">L’élément **Contains** représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.</span><span class="sxs-lookup"><span data-stu-id="fe419-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


<span data-ttu-id="fe419-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="fe419-105">**ContainsExpressionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fe419-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe419-106">Attributes and elements</span></span>

<span data-ttu-id="fe419-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe419-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe419-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe419-108">Attributes</span></span>

|<span data-ttu-id="fe419-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fe419-109">**Attribute**</span></span>|<span data-ttu-id="fe419-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe419-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe419-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="fe419-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="fe419-112">Identifie les limites d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="fe419-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="fe419-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="fe419-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="fe419-114">Détermine si la recherche ignore les cas et les espaces.</span><span class="sxs-lookup"><span data-stu-id="fe419-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="fe419-115">Valeurs d’attribut ContainmentMode</span><span class="sxs-lookup"><span data-stu-id="fe419-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="fe419-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fe419-116">**Value**</span></span>|<span data-ttu-id="fe419-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe419-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe419-118">FullString</span><span class="sxs-lookup"><span data-stu-id="fe419-118">FullString</span></span>  <br/> |<span data-ttu-id="fe419-119">La comparaison se fait entre la chaîne complète et la constante.</span><span class="sxs-lookup"><span data-stu-id="fe419-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="fe419-120">La valeur de la propriété et la constante fournie sont rigoureusement identiques.</span><span class="sxs-lookup"><span data-stu-id="fe419-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="fe419-121">Préfixe</span><span class="sxs-lookup"><span data-stu-id="fe419-121">Prefixed</span></span>  <br/> |<span data-ttu-id="fe419-122">La comparaison se fait entre le préfixe de chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="fe419-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="fe419-123">Sous-chaîne</span><span class="sxs-lookup"><span data-stu-id="fe419-123">Substring</span></span>  <br/> |<span data-ttu-id="fe419-124">La comparaison se fait entre une sous-chaîne de la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="fe419-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="fe419-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="fe419-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="fe419-126">La comparaison se fait entre un préfixe sur des mots individuels dans la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="fe419-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="fe419-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="fe419-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="fe419-128">La comparaison se fait entre une expression exacte dans la chaîne et la constante.</span><span class="sxs-lookup"><span data-stu-id="fe419-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="fe419-129">Valeurs d’attribut ContainmentComparison</span><span class="sxs-lookup"><span data-stu-id="fe419-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="fe419-130">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fe419-130">**Value**</span></span>|<span data-ttu-id="fe419-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe419-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe419-132">Orthographe</span><span class="sxs-lookup"><span data-stu-id="fe419-132">Exact</span></span>  <br/> |<span data-ttu-id="fe419-133">La comparaison doit être exacte.</span><span class="sxs-lookup"><span data-stu-id="fe419-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="fe419-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="fe419-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="fe419-135">La comparaison ne tient pas compte de la casse.</span><span class="sxs-lookup"><span data-stu-id="fe419-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="fe419-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="fe419-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="fe419-137">La comparaison ne tient pas compte des caractères non-espacement.</span><span class="sxs-lookup"><span data-stu-id="fe419-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="fe419-138">Espacé</span><span class="sxs-lookup"><span data-stu-id="fe419-138">Loose</span></span>  <br/> |<span data-ttu-id="fe419-139">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="fe419-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="fe419-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="fe419-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="fe419-141">La comparaison ne tient pas compte des caractères de casse et de non-espacement.</span><span class="sxs-lookup"><span data-stu-id="fe419-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="fe419-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="fe419-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="fe419-143">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="fe419-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="fe419-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="fe419-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="fe419-145">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="fe419-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="fe419-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="fe419-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="fe419-147">À supprimer.</span><span class="sxs-lookup"><span data-stu-id="fe419-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fe419-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe419-148">Child elements</span></span>

|<span data-ttu-id="fe419-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe419-149">**Element**</span></span>|<span data-ttu-id="fe419-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe419-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe419-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="fe419-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="fe419-152">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="fe419-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="fe419-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fe419-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="fe419-154">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="fe419-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="fe419-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fe419-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="fe419-156">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="fe419-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="fe419-157">Constante</span><span class="sxs-lookup"><span data-stu-id="fe419-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="fe419-158">Identifie une valeur constante dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="fe419-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe419-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe419-159">Parent elements</span></span>

|<span data-ttu-id="fe419-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe419-160">**Element**</span></span>|<span data-ttu-id="fe419-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe419-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe419-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="fe419-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="fe419-163">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="fe419-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="fe419-164">Not</span><span class="sxs-lookup"><span data-stu-id="fe419-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="fe419-165">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="fe419-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="fe419-166">And</span><span class="sxs-lookup"><span data-stu-id="fe419-166">And</span></span>](and.md) <br/> |<span data-ttu-id="fe419-167">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="fe419-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="fe419-168">Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.</span><span class="sxs-lookup"><span data-stu-id="fe419-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="fe419-169">Or</span><span class="sxs-lookup"><span data-stu-id="fe419-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="fe419-170">Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="fe419-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="fe419-171">L’élément [ou](or.md) renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="fe419-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fe419-172">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe419-172">Remarks</span></span>

<span data-ttu-id="fe419-173">Les attributs sont utilisés pour déterminer comment les éléments sont mis en correspondance.</span><span class="sxs-lookup"><span data-stu-id="fe419-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="fe419-174">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fe419-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe419-175">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe419-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe419-176">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe419-176">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe419-177">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe419-177">Schema Name</span></span>  <br/> |<span data-ttu-id="fe419-178">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fe419-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe419-179">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe419-179">Validation File</span></span>  <br/> |<span data-ttu-id="fe419-180">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fe419-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe419-181">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe419-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe419-182">False</span><span class="sxs-lookup"><span data-stu-id="fe419-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe419-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe419-183">See also</span></span>

- [<span data-ttu-id="fe419-184">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe419-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

