---
title: Utiliser des filtres de recherche avec EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Découvrez comment utiliser les filtres de recherche avec les API managées EWS dans Exchange.
ms.openlocfilehash: 0652c36fd610c2f9dfe22b55323b368997137e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754965"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="68056-103">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68056-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="68056-104">Découvrez comment utiliser les filtres de recherche avec les API managées EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="68056-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="68056-105">Filtres de recherche sont le principal outil pour exprimer des critères de recherche dans des applications EWS API managées.</span><span class="sxs-lookup"><span data-stu-id="68056-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="68056-106">Nous vous recommandons d’utiliser des filtres de recherche, au lieu de [chaînes de requête](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), pour effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="68056-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="68056-107">Recherche sur une propriété spécifique ou un ensemble de propriétés.</span><span class="sxs-lookup"><span data-stu-id="68056-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="68056-108">Recherche à l’aide de plusieurs critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="68056-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="68056-109">Filtres de recherche sont la seule option disponible si vous effectuez une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="68056-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="68056-110">Recherche des propriétés personnalisées.</span><span class="sxs-lookup"><span data-stu-id="68056-110">Searching custom properties.</span></span>  
- <span data-ttu-id="68056-111">Recherche de l’exécution d’une chaîne qui respecte la casse.</span><span class="sxs-lookup"><span data-stu-id="68056-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="68056-112">Exécution de préfixe ou chaîne exacte de recherche.</span><span class="sxs-lookup"><span data-stu-id="68056-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="68056-113">Recherche de l’exécution de masque de bits.</span><span class="sxs-lookup"><span data-stu-id="68056-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="68056-114">Recherche d’éléments dont la propriété spécifique défini, quelle que soit la valeur.</span><span class="sxs-lookup"><span data-stu-id="68056-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="68056-115">Recherche de dossiers.</span><span class="sxs-lookup"><span data-stu-id="68056-115">Searching for folders.</span></span>
- <span data-ttu-id="68056-116">Création de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="68056-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="68056-117">Déterminer le type de filtre de recherche que vous avez besoin</span><span class="sxs-lookup"><span data-stu-id="68056-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="68056-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-118"></span></span>

<span data-ttu-id="68056-119">Avant de créer un filtre de recherche, déterminez d’abord quel type de filtre que vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="68056-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="68056-120">Les types de filtres sont implémentées en tant que classes descendants de la classe [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) dans l’API managée EWS, ainsi que des éléments enfants de l’élément [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="68056-120">The filter types are implemented as descendant classes of the [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="68056-121">**Le tableau 1. Types de filtres de recherche**</span><span class="sxs-lookup"><span data-stu-id="68056-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="68056-122">**Type de filtre**</span><span class="sxs-lookup"><span data-stu-id="68056-122">**Filter type**</span></span>|<span data-ttu-id="68056-123">**Classe de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="68056-123">**EWS Managed API class**</span></span>|<span data-ttu-id="68056-124">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="68056-124">**EWS element**</span></span>|<span data-ttu-id="68056-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="68056-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="68056-126">Contient le filtre</span><span class="sxs-lookup"><span data-stu-id="68056-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="68056-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="68056-127">ContainsSubstring</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-128">Contient</span><span class="sxs-lookup"><span data-stu-id="68056-128">Contains</span></span>](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-129">Le meilleur type de filtre à utiliser pour les comparaisons de chaînes.</span><span class="sxs-lookup"><span data-stu-id="68056-129">The best filter type to use for string comparisons.</span></span> <span data-ttu-id="68056-130">Il permet de contrôler la casse, s’il faut ignorer l’espace blanc et définir le mode de contenance.</span><span class="sxs-lookup"><span data-stu-id="68056-130">It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="68056-131">Filtre de masque de bits</span><span class="sxs-lookup"><span data-stu-id="68056-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="68056-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="68056-132">ExcludesBitmask</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-133">Exclut</span><span class="sxs-lookup"><span data-stu-id="68056-133">Excludes</span></span>](http://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-134">Permet de vous permet de rechercher des propriétés des entiers comme masques de bits et retourner uniquement des résultats qui ont des bits correspondant à annuler le masque de bits spécifié.</span><span class="sxs-lookup"><span data-stu-id="68056-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="68056-135">Il existe de filtre</span><span class="sxs-lookup"><span data-stu-id="68056-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="68056-136">Exists</span><span class="sxs-lookup"><span data-stu-id="68056-136">Exists</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-137">Exists</span><span class="sxs-lookup"><span data-stu-id="68056-137">Exists</span></span>](http://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-138">Renvoie tous les éléments dont la propriété spécifiée existe, quelle que soit la valeur.</span><span class="sxs-lookup"><span data-stu-id="68056-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="68056-139">Filtre d’égalité</span><span class="sxs-lookup"><span data-stu-id="68056-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="68056-140">Plutôt IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-140">IsEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="68056-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-141">IsNotEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-142">Plutôt IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-142">IsEqualTo</span></span>](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="68056-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-143">IsNotEqualTo</span></span>](http://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-144">Compare la valeur de la propriété spécifiée avec une valeur de constante spécifiée ou la valeur d’une autre propriété et renvoyer tous les éléments qui ont une valeur égale (dans le cas d’un filtre **plutôt IsEqualTo** ) ou une valeur non égal (dans le cas d’un **IsNotEqualTo **filtre).</span><span class="sxs-lookup"><span data-stu-id="68056-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="68056-145">Filtre test relationnel</span><span class="sxs-lookup"><span data-stu-id="68056-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="68056-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="68056-146">IsGreaterThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="68056-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-147">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="68056-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="68056-148">IsLessThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="68056-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-149">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="68056-150">IsGreaterThan</span></span>](http://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="68056-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-151">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="68056-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="68056-152">IsLessThan</span></span>](http://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="68056-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="68056-153">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-154">Renvoie tous les éléments dont la valeur de la propriété spécifiée dans la relation appropriée à une valeur de constante spécifiée ou une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="68056-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="68056-155">Par exemple, un filtre **IsGreaterThan** renvoie tous les éléments dont la valeur est supérieure à la valeur spécifiée dans la propriété spécifiée.</span><span class="sxs-lookup"><span data-stu-id="68056-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="68056-156">Filtre une inversion</span><span class="sxs-lookup"><span data-stu-id="68056-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="68056-157">Pas</span><span class="sxs-lookup"><span data-stu-id="68056-157">Not</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-158">Pas</span><span class="sxs-lookup"><span data-stu-id="68056-158">Not</span></span>](http://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-159">Annule le résultat des autres filtres.</span><span class="sxs-lookup"><span data-stu-id="68056-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="68056-160">Filtre composé</span><span class="sxs-lookup"><span data-stu-id="68056-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="68056-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="68056-161">SearchFilterCollection</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="68056-162">And</span><span class="sxs-lookup"><span data-stu-id="68056-162">And</span></span>](http://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="68056-163">Or</span><span class="sxs-lookup"><span data-stu-id="68056-163">Or</span></span>](http://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="68056-164">Combine plusieurs filtres, permettant aux critères de recherche plus complexes.</span><span class="sxs-lookup"><span data-stu-id="68056-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="68056-165">Contient le filtre</span><span class="sxs-lookup"><span data-stu-id="68056-165">Contains filter</span></span>

<span data-ttu-id="68056-166">Contient un filtre est le meilleur choix pour la recherche des propriétés de type chaîne.</span><span class="sxs-lookup"><span data-stu-id="68056-166">A contains filter is the best choice for searching string properties.</span></span> <span data-ttu-id="68056-167">Avec un contient le filtre, vous pouvez contrôler les aspects de la correspondance de chaînes, telles que la casse et traitée espace blanc, en définissant le mode de contenance et le mode de comparaison.</span><span class="sxs-lookup"><span data-stu-id="68056-167">With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-168">Contient le filtre dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="68056-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-169"></span></span>

<span data-ttu-id="68056-170">Si vous utilisez l’API managée EWS, vous définissez le mode de relation contenant-contenu à l’aide de la propriété [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) de la classe [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) , et vous définissez le mode de comparaison à l’aide de la propriété [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) de la ** ContainsSubstring** classe.</span><span class="sxs-lookup"><span data-stu-id="68056-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="68056-171">L’exemple suivant montre comment créer un filtre de recherche qui recherche dans le champ objet d’éléments de la sous-chaîne « notes de réunion ».</span><span class="sxs-lookup"><span data-stu-id="68056-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="68056-172">Cet exemple montre comment ignore la casse, mais n’ignore pas les espaces blancs.</span><span class="sxs-lookup"><span data-stu-id="68056-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="68056-173">Contient le filtre dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-173">Contains filter in EWS</span></span>
<span data-ttu-id="68056-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-174"></span></span>

<span data-ttu-id="68056-175">Vous définissez le mode de relation contenant-contenu à l’aide de l’attribut **ContainmentMode** sur l’élément [contient](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) dans EWS, et vous définissez le mode de comparaison à l’aide de l’attribut **ContainmentComparison** sur l’élément **contient** .</span><span class="sxs-lookup"><span data-stu-id="68056-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="68056-176">L’exemple suivant montre comment créer un filtre de recherche pour rechercher le champ objet d’éléments de la sous-chaîne « notes de réunion ».</span><span class="sxs-lookup"><span data-stu-id="68056-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="68056-177">Cet exemple montre comment ignore la casse, mais n’ignore pas les espaces blancs.</span><span class="sxs-lookup"><span data-stu-id="68056-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="68056-178">Filtre de masque de bits</span><span class="sxs-lookup"><span data-stu-id="68056-178">Bitmask filter</span></span>

<span data-ttu-id="68056-179">Un filtre de masque de bits vous permet de rechercher propriétés entier en tant que masques de bits et renvoyer des résultats où des bits spécifiques ne sont pas définis dans la valeur de la propriété spécifiée.</span><span class="sxs-lookup"><span data-stu-id="68056-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-180">Filtre de masque de bits dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-181">L’exemple suivant vous montre comment utiliser l’API managée EWS pour créer un filtre de recherche pour retourner tous les éléments qui ont une valeur dans la propriété personnalisée **ItemIndex** (définie dans le [exemple : rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS](#bk_ExampleEWSMA) section de cet article) qui n’ont pas le deuxième bit (10 en binaire) définie.</span><span class="sxs-lookup"><span data-stu-id="68056-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="68056-182">Filtre de masque de bits dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="68056-183">L’exemple suivant vous montre comment utiliser EWS pour créer un filtre de recherche pour retourner tous les éléments qui ont une valeur dans la propriété personnalisée **ItemIndex** (définie dans le [exemple : rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS](#bk_ExampleEWSMA) section de cet article) qui n’ont pas le deuxième bit (10 en binaire) définie.</span><span class="sxs-lookup"><span data-stu-id="68056-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="68056-184">Il existe de filtre</span><span class="sxs-lookup"><span data-stu-id="68056-184">Exists filter</span></span>

<span data-ttu-id="68056-185">Un existe filtre vous permet de rechercher des éléments qui ont une propriété spécifique, indépendamment de la valeur.</span><span class="sxs-lookup"><span data-stu-id="68056-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-186">Il existe de filtre dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-187">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments dont la propriété personnalisée **ItemIndex** défini.</span><span class="sxs-lookup"><span data-stu-id="68056-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="68056-188">Il existe de filtre dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-188">Exists filter in EWS</span></span>

<span data-ttu-id="68056-189">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments dont la propriété personnalisée **ItemIndex** défini.</span><span class="sxs-lookup"><span data-stu-id="68056-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="68056-190">Filtre d’égalité</span><span class="sxs-lookup"><span data-stu-id="68056-190">Equality filter</span></span>

<span data-ttu-id="68056-191">Filtres d’égalité permettent de rechercher tous les éléments dont la valeur de la propriété spécifiée est égale à une valeur spécifique ou une valeur spécifique est différent.</span><span class="sxs-lookup"><span data-stu-id="68056-191">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value.</span></span> <span data-ttu-id="68056-192">La valeur à comparer avec peut être une valeur constante ou la valeur d’une autre propriété sur chaque élément.</span><span class="sxs-lookup"><span data-stu-id="68056-192">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-193">Filtre d’égalité dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-194">L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche pour retourner tous les éléments qui n’ont pas été lus.</span><span class="sxs-lookup"><span data-stu-id="68056-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="68056-195">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments qui ont une valeur dans la propriété **ItemIndex** qui n’est pas égale à la taille de l’élément.</span><span class="sxs-lookup"><span data-stu-id="68056-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="68056-196">Filtre d’égalité dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-196">Equality filter in EWS</span></span>

<span data-ttu-id="68056-197">L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche pour retourner tous les éléments qui n’ont pas été lus.</span><span class="sxs-lookup"><span data-stu-id="68056-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="68056-198">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments qui ont une valeur dans la propriété **ItemIndex** qui n’est pas égale à la taille de l’élément.</span><span class="sxs-lookup"><span data-stu-id="68056-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="68056-199">Filtre test relationnel</span><span class="sxs-lookup"><span data-stu-id="68056-199">Relational testing filter</span></span>

<span data-ttu-id="68056-200">Filtres tests relationnelles permettent de rechercher tous les éléments dont la valeur de la propriété spécifiée est supérieure à (\>), supérieur ou égal à (\>=), inférieur à (\<), ou inférieure ou égale à (\<=) une valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="68056-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="68056-201">La valeur à comparer avec peut être une valeur constante ou la valeur d’une autre propriété sur chaque élément.</span><span class="sxs-lookup"><span data-stu-id="68056-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-202">Filtre de test relationnel dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-203">L’exemple suivant montre comment utiliser l’API managée EWS pour créer des filtres de recherche pour renvoyer tous les éléments dont la valeur de la propriété **ItemIndex** dont la relation spécifiée avec la valeur de constante 3.</span><span class="sxs-lookup"><span data-stu-id="68056-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="68056-204">Filtre de test relationnel dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="68056-205">L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche pour renvoyer tous les éléments dont la valeur de la propriété **ItemIndex** est supérieure à la valeur de constante 3.</span><span class="sxs-lookup"><span data-stu-id="68056-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="68056-206">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments avec une valeur dans la propriété **ItemIndex** qui est supérieure ou égale à la valeur de constante 3.</span><span class="sxs-lookup"><span data-stu-id="68056-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="68056-207">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments avec une valeur dans la propriété **ItemIndex** qui est inférieure à la valeur de constante 3.</span><span class="sxs-lookup"><span data-stu-id="68056-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="68056-208">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments avec une valeur dans la propriété **ItemIndex** qui est inférieure ou égale à la valeur de constante 3.</span><span class="sxs-lookup"><span data-stu-id="68056-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="68056-209">Filtre une inversion</span><span class="sxs-lookup"><span data-stu-id="68056-209">Negating filter</span></span>

<span data-ttu-id="68056-210">Un filtre une inversion permet d’annuler un autre filtre et obtenir les résultats de recherche inverse.</span><span class="sxs-lookup"><span data-stu-id="68056-210">A negating filter enables you to negate another filter and get the opposite search results.</span></span> <span data-ttu-id="68056-211">Alors que les autres filtres de renvoyer des résultats qui correspondent à des critères spécifiques, un filtre une inversion renvoie des résultats qui ne correspondent pas aux critères spécifiés par le filtre, à qu'elle est appliquée.</span><span class="sxs-lookup"><span data-stu-id="68056-211">While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-212">Filtre une inversion dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-213">L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche pour retourner tous les éléments qui n’ont pas la sous-chaîne « notes de réunion » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="68056-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="68056-214">Filtre une inversion dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-214">Negating filter in EWS</span></span>

<span data-ttu-id="68056-215">L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments qui n’ont pas la sous-chaîne « notes de réunion » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="68056-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="68056-216">Filtre composé</span><span class="sxs-lookup"><span data-stu-id="68056-216">Compound filter</span></span>

<span data-ttu-id="68056-217">Un filtre composé vous permet de combiner plusieurs filtres pour créer des critères de recherche plus complexes.</span><span class="sxs-lookup"><span data-stu-id="68056-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="68056-218">Vous pouvez combiner les critères à l’aide des opérateurs logiques et ou ou.</span><span class="sxs-lookup"><span data-stu-id="68056-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="68056-219">De cette manière, vous pouvez effectuer les recherches comme « tous les messages à partir de Sadie Daniels qui contient les notes de réunion dans l’objet ».</span><span class="sxs-lookup"><span data-stu-id="68056-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="68056-220">Filtre composé dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="68056-221">L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche qui retourne tous les éléments qui sont envoyés à partir de Sadie Daniels et contiennent des « notes de réunion » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="68056-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="68056-222">Filtre composé dans EWS</span><span class="sxs-lookup"><span data-stu-id="68056-222">Compound filter in EWS</span></span>

<span data-ttu-id="68056-223">L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche qui retourne tous les éléments qui sont envoyés à partir de Sadie Daniels et qui contiennent des « notes de réunion » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="68056-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="68056-224">Exemple : Rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="68056-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="68056-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-225"></span></span>

<span data-ttu-id="68056-226">Les méthodes API managées suivantes utilisent des filtres de recherche :</span><span class="sxs-lookup"><span data-stu-id="68056-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="68056-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="68056-227">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="68056-228">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="68056-228">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="68056-229">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="68056-229">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="68056-230">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="68056-230">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="68056-231">L’exemple suivant utilise la méthode **ExchangeService.FindItems** ; Toutefois, les mêmes règles et concepts s’appliquent à toutes les méthodes.</span><span class="sxs-lookup"><span data-stu-id="68056-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="68056-232">Dans cet exemple, une méthode appelée **SearchWithFilter** est définie.</span><span class="sxs-lookup"><span data-stu-id="68056-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="68056-233">Il prend un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) en tant que paramètres.</span><span class="sxs-lookup"><span data-stu-id="68056-233">It takes an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="68056-234">Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="68056-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="68056-235">La classe **SearchFilter** est la classe de base pour tous les filtres de recherche.</span><span class="sxs-lookup"><span data-stu-id="68056-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="68056-236">Vous pouvez utiliser cette fonction avec un des filtres de recherche dans les exemples dans cet article.</span><span class="sxs-lookup"><span data-stu-id="68056-236">You can use this function with any of the search filters shown in the examples in this article.</span></span> <span data-ttu-id="68056-237">Cet exemple utilise un filtre composé pour renvoyer tous les éléments dans la boîte de réception à partir de Sadie Daniels avec « notes de réunion » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="68056-237">This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="68056-238">Exemple : Rechercher un élément en utilisant un filtre de recherche et les EWS</span><span class="sxs-lookup"><span data-stu-id="68056-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="68056-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-239"></span></span>

<span data-ttu-id="68056-240">Les opérations EWS suivantes utilisent des filtres de recherche :</span><span class="sxs-lookup"><span data-stu-id="68056-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="68056-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="68056-241">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="68056-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="68056-242">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="68056-243">L’exemple suivant utilise l’opération **FindItem** ; Toutefois, les mêmes règles et concepts s’appliquent à ces deux opérations.</span><span class="sxs-lookup"><span data-stu-id="68056-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="68056-244">Filtres de recherche sont contenues dans l’élément [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) dans les demandes SOAP.</span><span class="sxs-lookup"><span data-stu-id="68056-244">Search filters are contained in the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="68056-245">Cet exemple envoie une demande SOAP qui est équivalente à la recherche est illustrée dans l’exemple précédent API managées.</span><span class="sxs-lookup"><span data-stu-id="68056-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="68056-246">L’exemple suivant montre la réponse du serveur, y compris les résultats de recherche.</span><span class="sxs-lookup"><span data-stu-id="68056-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="68056-247">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="68056-247">Next steps</span></span>
<span data-ttu-id="68056-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="68056-248"></span></span>

<span data-ttu-id="68056-249">Maintenant que vous êtes familiarisé avec l’utilisation de filtres de recherche dans les recherches de base, vous pouvez déplacer sur les techniques de recherche avancées.</span><span class="sxs-lookup"><span data-stu-id="68056-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="68056-250">Effectuer des recherches groupées à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68056-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="68056-251">Effectuer des recherches paginées à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68056-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="68056-252">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="68056-252">See also</span></span>

- [<span data-ttu-id="68056-253">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68056-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="68056-254">Effectuer une recherche AQS à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68056-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="68056-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="68056-255">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="68056-256">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="68056-256">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="68056-257">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="68056-257">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="68056-258">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="68056-258">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="68056-259">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="68056-259">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="68056-260">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="68056-260">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

