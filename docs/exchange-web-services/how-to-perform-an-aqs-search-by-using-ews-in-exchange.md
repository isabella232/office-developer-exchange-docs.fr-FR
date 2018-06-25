---
title: Effectuer une recherche AQS à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Découvrez comment rechercher des chaînes de requête AQS dans des applications EWS API managées.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754939"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="6257d-103">Effectuer une recherche AQS à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6257d-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="6257d-104">Découvrez comment rechercher des chaînes de requête AQS dans des applications EWS API managées.</span><span class="sxs-lookup"><span data-stu-id="6257d-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="6257d-105">Chaînes de requête constituent une alternative aux [filtres de recherche](how-to-use-search-filters-with-ews-in-exchange.md) pour l’expression de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="6257d-106">Le principal avantage de chaînes de requête est que vous devez pas spécifier une propriété unique pour la recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="6257d-107">Vous pouvez fournir simplement une valeur et la recherche s’appliquent à tous les champs couramment utilisées sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="6257d-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="6257d-108">Vous pouvez également affiner votre recherche à l’aide de la syntaxe de requête avancée (AQS) au lieu d’une valeur simple.</span><span class="sxs-lookup"><span data-stu-id="6257d-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="6257d-109">Toutefois, les chaînes de requête ont les limitations suivantes que vous devez connaître avant de les ajouter à votre boîte à outils :</span><span class="sxs-lookup"><span data-stu-id="6257d-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="6257d-110">**Capacité limitée à rechercher des propriétés spécifiques.**</span><span class="sxs-lookup"><span data-stu-id="6257d-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="6257d-111">Lorsque vous recherchez avec une valeur dans une chaîne de requête simple, la recherche est effectuée sur toutes les propriétés indexées.</span><span class="sxs-lookup"><span data-stu-id="6257d-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="6257d-112">Vous pouvez affiner la recherche à des propriétés spécifiques, mais les propriétés disponibles pour une utilisation dans une chaîne AQS sont limitées.</span><span class="sxs-lookup"><span data-stu-id="6257d-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="6257d-113">Si la propriété que vous souhaitez rechercher n’est pas une des propriétés qui sont disponibles pour AQS, envisagez d’utiliser un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="6257d-114">**Propriétés personnalisées ne sont pas recherchées.**</span><span class="sxs-lookup"><span data-stu-id="6257d-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="6257d-115">Les recherches de chaînes de requête sont effectuées par rapport à un index et des propriétés personnalisées ne sont pas incluses dans cet index.</span><span class="sxs-lookup"><span data-stu-id="6257d-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="6257d-116">Si vous avez besoin rechercher des propriétés personnalisées, utilisez plutôt un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="6257d-117">**Contrôle limité pour la chaîne de recherche.**</span><span class="sxs-lookup"><span data-stu-id="6257d-117">**Limited control for string searches.**</span></span> <span data-ttu-id="6257d-118">Les recherches de chaînes de requête toujours ignorent la casse et sont toujours des recherches de sous-chaînes.</span><span class="sxs-lookup"><span data-stu-id="6257d-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="6257d-119">Si vous souhaitez faire la casse, préfixe ou les recherches de concordance exacte, utilisent un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="6257d-120">**Non disponible pour les dossiers ou les dossiers de recherche.**</span><span class="sxs-lookup"><span data-stu-id="6257d-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="6257d-121">Les opérations EWS pour la recherche de dossiers ne prend pas en charge à l’aide d’une chaîne de requête.</span><span class="sxs-lookup"><span data-stu-id="6257d-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="6257d-122">En outre, les dossiers de recherche ne prennent en charge les chaînes de requête.</span><span class="sxs-lookup"><span data-stu-id="6257d-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="6257d-123">Dans les deux cas, un filtre de recherche est la seule option.</span><span class="sxs-lookup"><span data-stu-id="6257d-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="6257d-124">Création d’une chaîne de requête</span><span class="sxs-lookup"><span data-stu-id="6257d-124">Creating a query string</span></span>
<span data-ttu-id="6257d-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="6257d-125"></span></span>

<span data-ttu-id="6257d-126">Chaînes de requête dans les API managées EWS sont interprétées comme un sous-ensemble de la syntaxe AQS.</span><span class="sxs-lookup"><span data-stu-id="6257d-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="6257d-127">Chaînes AQS sont composés des valeurs ou paires mot clé/valeur, séparées par un signe deux-points ( :)).</span><span class="sxs-lookup"><span data-stu-id="6257d-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="6257d-128">Lorsqu’une valeur est spécifiée sans un mot clé, la valeur sont recherchées dans toutes les propriétés indexées.</span><span class="sxs-lookup"><span data-stu-id="6257d-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="6257d-129">Si un mot clé est associé à une valeur, le mot clé spécifie une propriété pour rechercher la valeur correspondante.</span><span class="sxs-lookup"><span data-stu-id="6257d-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="6257d-130">**Le tableau 1. Mots-clés AQS pris en charge**</span><span class="sxs-lookup"><span data-stu-id="6257d-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="6257d-131">**Mot clé**</span><span class="sxs-lookup"><span data-stu-id="6257d-131">**Keyword**</span></span>|<span data-ttu-id="6257d-132">**Type de valeur**</span><span class="sxs-lookup"><span data-stu-id="6257d-132">**Value type**</span></span>|<span data-ttu-id="6257d-133">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="6257d-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6257d-134">subject</span><span class="sxs-lookup"><span data-stu-id="6257d-134">subject</span></span>  <br/> |<span data-ttu-id="6257d-135">String</span><span class="sxs-lookup"><span data-stu-id="6257d-135">String</span></span>  <br/> |<span data-ttu-id="6257d-136">objet : project</span><span class="sxs-lookup"><span data-stu-id="6257d-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="6257d-137">body</span><span class="sxs-lookup"><span data-stu-id="6257d-137">body</span></span>  <br/> |<span data-ttu-id="6257d-138">String</span><span class="sxs-lookup"><span data-stu-id="6257d-138">String</span></span>  <br/> |<span data-ttu-id="6257d-139">illustrations de corps : ventes</span><span class="sxs-lookup"><span data-stu-id="6257d-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="6257d-140">pièce jointe</span><span class="sxs-lookup"><span data-stu-id="6257d-140">attachment</span></span>  <br/> |<span data-ttu-id="6257d-141">String</span><span class="sxs-lookup"><span data-stu-id="6257d-141">String</span></span>  <br/> |<span data-ttu-id="6257d-142">pièce jointe : état</span><span class="sxs-lookup"><span data-stu-id="6257d-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="6257d-143">et utilisez à la place</span><span class="sxs-lookup"><span data-stu-id="6257d-143">to</span></span>  <br/> |<span data-ttu-id="6257d-144">String</span><span class="sxs-lookup"><span data-stu-id="6257d-144">String</span></span>  <br/> |<span data-ttu-id="6257d-145">à : « Sadie danield »</span><span class="sxs-lookup"><span data-stu-id="6257d-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="6257d-146">from</span><span class="sxs-lookup"><span data-stu-id="6257d-146">from</span></span>  <br/> |<span data-ttu-id="6257d-147">String</span><span class="sxs-lookup"><span data-stu-id="6257d-147">String</span></span>  <br/> |<span data-ttu-id="6257d-148">à partir de : espère que</span><span class="sxs-lookup"><span data-stu-id="6257d-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="6257d-149">cc</span><span class="sxs-lookup"><span data-stu-id="6257d-149">cc</span></span>  <br/> |<span data-ttu-id="6257d-150">String</span><span class="sxs-lookup"><span data-stu-id="6257d-150">String</span></span>  <br/> |<span data-ttu-id="6257d-151">cc : « Ronnie Sturgis »</span><span class="sxs-lookup"><span data-stu-id="6257d-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="6257d-152">bcc</span><span class="sxs-lookup"><span data-stu-id="6257d-152">bcc</span></span>  <br/> |<span data-ttu-id="6257d-153">String</span><span class="sxs-lookup"><span data-stu-id="6257d-153">String</span></span>  <br/> |<span data-ttu-id="6257d-154">Bcc:Mack</span><span class="sxs-lookup"><span data-stu-id="6257d-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="6257d-155">participants</span><span class="sxs-lookup"><span data-stu-id="6257d-155">participants</span></span>  <br/> |<span data-ttu-id="6257d-156">String</span><span class="sxs-lookup"><span data-stu-id="6257d-156">String</span></span>  <br/> |<span data-ttu-id="6257d-157">participants : sadie</span><span class="sxs-lookup"><span data-stu-id="6257d-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="6257d-158">catégorie</span><span class="sxs-lookup"><span data-stu-id="6257d-158">category</span></span>  <br/> |<span data-ttu-id="6257d-159">String</span><span class="sxs-lookup"><span data-stu-id="6257d-159">String</span></span>  <br/> |<span data-ttu-id="6257d-160">catégorie : projet</span><span class="sxs-lookup"><span data-stu-id="6257d-160">category:project</span></span>  <br/> |
|<span data-ttu-id="6257d-161">importance</span><span class="sxs-lookup"><span data-stu-id="6257d-161">importance</span></span>  <br/> |<span data-ttu-id="6257d-162">String</span><span class="sxs-lookup"><span data-stu-id="6257d-162">String</span></span>  <br/> |<span data-ttu-id="6257d-163">importance : haute</span><span class="sxs-lookup"><span data-stu-id="6257d-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="6257d-164">type</span><span class="sxs-lookup"><span data-stu-id="6257d-164">kind</span></span>  <br/> |<span data-ttu-id="6257d-165">Type d’élément</span><span class="sxs-lookup"><span data-stu-id="6257d-165">Item type</span></span>  <br/> |<span data-ttu-id="6257d-166">type : réunions</span><span class="sxs-lookup"><span data-stu-id="6257d-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="6257d-167">envoyé</span><span class="sxs-lookup"><span data-stu-id="6257d-167">sent</span></span>  <br/> |<span data-ttu-id="6257d-168">Date</span><span class="sxs-lookup"><span data-stu-id="6257d-168">Date</span></span>  <br/> |<span data-ttu-id="6257d-169">envoyés : 10/12/2013</span><span class="sxs-lookup"><span data-stu-id="6257d-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="6257d-170">reçus</span><span class="sxs-lookup"><span data-stu-id="6257d-170">received</span></span>  <br/> |<span data-ttu-id="6257d-171">Date</span><span class="sxs-lookup"><span data-stu-id="6257d-171">Date</span></span>  <br/> |<span data-ttu-id="6257d-172">reçus : hier</span><span class="sxs-lookup"><span data-stu-id="6257d-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="6257d-173">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="6257d-173">hasattachment</span></span>  <br/> |<span data-ttu-id="6257d-174">Bool�en</span><span class="sxs-lookup"><span data-stu-id="6257d-174">Boolean</span></span>  <br/> |<span data-ttu-id="6257d-175">Possède des pièces jointes : true</span><span class="sxs-lookup"><span data-stu-id="6257d-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="6257d-176">est marqué</span><span class="sxs-lookup"><span data-stu-id="6257d-176">isflagged</span></span>  <br/> |<span data-ttu-id="6257d-177">Bool�en</span><span class="sxs-lookup"><span data-stu-id="6257d-177">Boolean</span></span>  <br/> |<span data-ttu-id="6257d-178">isflagged:true</span><span class="sxs-lookup"><span data-stu-id="6257d-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="6257d-179">estlu</span><span class="sxs-lookup"><span data-stu-id="6257d-179">isread</span></span>  <br/> |<span data-ttu-id="6257d-180">Bool�en</span><span class="sxs-lookup"><span data-stu-id="6257d-180">Boolean</span></span>  <br/> |<span data-ttu-id="6257d-181">isread:False</span><span class="sxs-lookup"><span data-stu-id="6257d-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="6257d-182">size</span><span class="sxs-lookup"><span data-stu-id="6257d-182">size</span></span>  <br/> |<span data-ttu-id="6257d-183">Nombre</span><span class="sxs-lookup"><span data-stu-id="6257d-183">Number</span></span>  <br/> |<span data-ttu-id="6257d-184">taille :\>5000</span><span class="sxs-lookup"><span data-stu-id="6257d-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="6257d-185">Examinons comment fonctionnent les types de valeurs différents.</span><span class="sxs-lookup"><span data-stu-id="6257d-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="6257d-186">À l’aide d’une valeur de type chaîne</span><span class="sxs-lookup"><span data-stu-id="6257d-186">Using a string value type</span></span>

<span data-ttu-id="6257d-187">Types de valeur de chaîne sont par défaut exclu en tant que les recherches de sous-chaînes préfixe qui ne respectent pas la casse.</span><span class="sxs-lookup"><span data-stu-id="6257d-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="6257d-188">Cela signifie que recherche d’objet : projet renverrait des sujets suivants :</span><span class="sxs-lookup"><span data-stu-id="6257d-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="6257d-189">Notes de la réunion de projet</span><span class="sxs-lookup"><span data-stu-id="6257d-189">Project meeting notes</span></span>
    
- <span data-ttu-id="6257d-190">Avez-vous besoin des plans de projet ?</span><span class="sxs-lookup"><span data-stu-id="6257d-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="6257d-191">Prévisions de ventes décembre</span><span class="sxs-lookup"><span data-stu-id="6257d-191">December sales projections</span></span>
    
<span data-ttu-id="6257d-192">Vous pouvez modifier la recherche pour exiger que le mot entier plutôt que de correspondance de préfixes, en mettant la chaîne entre guillemets.</span><span class="sxs-lookup"><span data-stu-id="6257d-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="6257d-193">Recherche de l’objet : « projet » élimine la valeur « Prévisions de ventes décembre » dans la liste des correspondances.</span><span class="sxs-lookup"><span data-stu-id="6257d-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="6257d-194">Notez que la valeur est toujours pas la casse.</span><span class="sxs-lookup"><span data-stu-id="6257d-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="6257d-195">Si vous utilisez plusieurs mots dans une chaîne de requête, une correspondance nécessite que les mots apparaissent dans les champs de recherches.</span><span class="sxs-lookup"><span data-stu-id="6257d-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="6257d-196">Par exemple, recherche d’objet : projet renverrait des sujets suivants :</span><span class="sxs-lookup"><span data-stu-id="6257d-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="6257d-197">Plan de projet</span><span class="sxs-lookup"><span data-stu-id="6257d-197">Project plan</span></span>
    
- <span data-ttu-id="6257d-198">Avez-vous besoin des plans de projet ?</span><span class="sxs-lookup"><span data-stu-id="6257d-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="6257d-199">Envoyez-moi le plan de projet</span><span class="sxs-lookup"><span data-stu-id="6257d-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="6257d-200">Planification des jalons du projet</span><span class="sxs-lookup"><span data-stu-id="6257d-200">Planning project milestones</span></span>
    
<span data-ttu-id="6257d-201">Si vous placez plusieurs mots entre guillemets, ils sont considérés comme une seule phrase.</span><span class="sxs-lookup"><span data-stu-id="6257d-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="6257d-202">Recherche de l’objet : « projet » renverrait uniquement l’objet « Projet » de la liste précédente.</span><span class="sxs-lookup"><span data-stu-id="6257d-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="6257d-203">À l’aide d’un type de valeur de type élément</span><span class="sxs-lookup"><span data-stu-id="6257d-203">Using an item type value type</span></span>

<span data-ttu-id="6257d-204">Vous pouvez utiliser les valeurs de type d’élément suivantes avec le mot clé **type** pour limiter vos résultats de recherche à uniquement un type spécifique d’élément, tel que courrier ou les demandes de réunion :</span><span class="sxs-lookup"><span data-stu-id="6257d-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="6257d-205">contacts</span><span class="sxs-lookup"><span data-stu-id="6257d-205">contacts</span></span>    
- <span data-ttu-id="6257d-206">documents</span><span class="sxs-lookup"><span data-stu-id="6257d-206">docs</span></span>    
- <span data-ttu-id="6257d-207">email</span><span class="sxs-lookup"><span data-stu-id="6257d-207">email</span></span>    
- <span data-ttu-id="6257d-208">télécopies</span><span class="sxs-lookup"><span data-stu-id="6257d-208">faxes</span></span>    
- <span data-ttu-id="6257d-209">messagerie instantanée (correspond aux messages instantanés)</span><span class="sxs-lookup"><span data-stu-id="6257d-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="6257d-210">feuilles</span><span class="sxs-lookup"><span data-stu-id="6257d-210">journals</span></span>    
- <span data-ttu-id="6257d-211">réunions (correspond au rendez-vous et demandes de réunion)</span><span class="sxs-lookup"><span data-stu-id="6257d-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="6257d-212">notes</span><span class="sxs-lookup"><span data-stu-id="6257d-212">notes</span></span>    
- <span data-ttu-id="6257d-213">posts</span><span class="sxs-lookup"><span data-stu-id="6257d-213">posts</span></span>    
- <span data-ttu-id="6257d-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="6257d-214">rssfeeds</span></span>    
- <span data-ttu-id="6257d-215">tasks</span><span class="sxs-lookup"><span data-stu-id="6257d-215">tasks</span></span>    
- <span data-ttu-id="6257d-216">messagerie vocale</span><span class="sxs-lookup"><span data-stu-id="6257d-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="6257d-217">À l’aide d’un type de valeur de date</span><span class="sxs-lookup"><span data-stu-id="6257d-217">Using a date value type</span></span>

<span data-ttu-id="6257d-218">Vous pouvez rechercher des types de valeur de date dans un certain nombre de différentes manières.</span><span class="sxs-lookup"><span data-stu-id="6257d-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="6257d-219">Est la plus simple pour rechercher une date spécifique.</span><span class="sxs-lookup"><span data-stu-id="6257d-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="6257d-220">Recherche avec reçus : 12/11/2013 retournera tous les éléments reçus sur le 11 décembre 2013.</span><span class="sxs-lookup"><span data-stu-id="6257d-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="6257d-221">Toutefois, vous pouvez également être moins spécifique.</span><span class="sxs-lookup"><span data-stu-id="6257d-221">However, you can also be less specific.</span></span> <span data-ttu-id="6257d-222">Recherche avec reçus : 12/11 retournera tous les éléments reçus sur le 11 décembre de l’année en cours.</span><span class="sxs-lookup"><span data-stu-id="6257d-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="6257d-223">Une autre option consiste à utiliser les noms de mois.</span><span class="sxs-lookup"><span data-stu-id="6257d-223">Another option is to use the month names.</span></span> <span data-ttu-id="6257d-224">Vous pouvez rechercher avec reçus : le 11 décembre 2013 ou 11 décembre pour obtenir les mêmes résultats reçues : 12/11/2013 et reçus : 12/11, respectivement.</span><span class="sxs-lookup"><span data-stu-id="6257d-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="6257d-225">Vous pouvez également rechercher avec reçus : décembre pour obtenir tous les éléments reçus dans le mois de décembre, l’année en cours.</span><span class="sxs-lookup"><span data-stu-id="6257d-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="6257d-226">Les noms des jours de la semaine est également une option.</span><span class="sxs-lookup"><span data-stu-id="6257d-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="6257d-227">Recherche avec reçus : Mardi retournera tous les éléments reçus mardi de la semaine en cours.</span><span class="sxs-lookup"><span data-stu-id="6257d-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="6257d-228">Types de valeur de date prennent également en charge un ensemble de mots clés pour les recherches par rapport à l’heure actuelle.</span><span class="sxs-lookup"><span data-stu-id="6257d-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="6257d-229">Les mots clés suivants sont pris en charge :</span><span class="sxs-lookup"><span data-stu-id="6257d-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="6257d-230">aujourd’hui</span><span class="sxs-lookup"><span data-stu-id="6257d-230">today</span></span>  
- <span data-ttu-id="6257d-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="6257d-231">tomorrow</span></span>
- <span data-ttu-id="6257d-232">yesterday</span><span class="sxs-lookup"><span data-stu-id="6257d-232">yesterday</span></span>
- <span data-ttu-id="6257d-233">this week</span><span class="sxs-lookup"><span data-stu-id="6257d-233">this week</span></span>    
- <span data-ttu-id="6257d-234">La semaine dernière</span><span class="sxs-lookup"><span data-stu-id="6257d-234">last week</span></span>    
- <span data-ttu-id="6257d-235">mois suivant</span><span class="sxs-lookup"><span data-stu-id="6257d-235">next month</span></span>    
- <span data-ttu-id="6257d-236">dernier mois</span><span class="sxs-lookup"><span data-stu-id="6257d-236">past month</span></span>    
- <span data-ttu-id="6257d-237">année à venir</span><span class="sxs-lookup"><span data-stu-id="6257d-237">coming year</span></span>
    
<span data-ttu-id="6257d-238">Types de valeur de date peuvent également être comparées aux opérateurs relationnels comme supérieur ou inférieur à, ou une plage avec l’opérateur de plage **.**. Par exemple, reçu :\>30/11/2013, envoyés :\>= hier, et received:12/1/2013..today sont toutes les chaînes de requête valide.</span><span class="sxs-lookup"><span data-stu-id="6257d-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="6257d-239">À l’aide d’un type de valeur de type Boolean</span><span class="sxs-lookup"><span data-stu-id="6257d-239">Using a Boolean value type</span></span>

<span data-ttu-id="6257d-240">Types de valeur de type Boolean peuvent être « true » ou « false ».</span><span class="sxs-lookup"><span data-stu-id="6257d-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="6257d-241">Les valeurs ne respectent pas la casse, donc isread:false produira les mêmes résultats qu’isread:FALSE.</span><span class="sxs-lookup"><span data-stu-id="6257d-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="6257d-242">À l’aide d’un type de valeur numérique</span><span class="sxs-lookup"><span data-stu-id="6257d-242">Using a number value type</span></span>

<span data-ttu-id="6257d-243">Types de valeur numériques peuvent être recherchées correspondances exactes, mais ils peuvent également être recherchés à l’aide des opérateurs relationnels comme supérieur ou inférieur à.</span><span class="sxs-lookup"><span data-stu-id="6257d-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="6257d-244">Par exemple, taille : 10000 retourne uniquement les éléments qui ont une taille d’exactement 10 000 octets, mais la taille :\>= 10000 renvoie les éléments qui ont une taille supérieure ou égale à 10 000 octets.</span><span class="sxs-lookup"><span data-stu-id="6257d-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="6257d-245">Vous pouvez également spécifier une plage à l’aide de l’opérateur de plage ( **.**).</span><span class="sxs-lookup"><span data-stu-id="6257d-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="6257d-246">Par exemple, taille : 7000..8000 renvoie les éléments qui ont une taille comprise entre 7000 et 8000.</span><span class="sxs-lookup"><span data-stu-id="6257d-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="6257d-247">Utilisation d’opérateurs logiques</span><span class="sxs-lookup"><span data-stu-id="6257d-247">Using logical operators</span></span>

<span data-ttu-id="6257d-248">Chaînes de requête prend en charge les opérateurs logiques suivants.</span><span class="sxs-lookup"><span data-stu-id="6257d-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="6257d-249">**Le tableau 2. Prise en charge des opérateurs logiques**</span><span class="sxs-lookup"><span data-stu-id="6257d-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="6257d-250">**Opérateur**</span><span class="sxs-lookup"><span data-stu-id="6257d-250">**Operator**</span></span>|<span data-ttu-id="6257d-251">**Exemples**</span><span class="sxs-lookup"><span data-stu-id="6257d-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6257d-252">AND</span><span class="sxs-lookup"><span data-stu-id="6257d-252">AND</span></span>  <br/> |<span data-ttu-id="6257d-253">projet et à partir de : « Sadie Daniels »</span><span class="sxs-lookup"><span data-stu-id="6257d-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="6257d-254">objet :(project AND plan)</span><span class="sxs-lookup"><span data-stu-id="6257d-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="6257d-255">OU</span><span class="sxs-lookup"><span data-stu-id="6257d-255">OR</span></span>  <br/> |<span data-ttu-id="6257d-256">objet : réunion ou à partir de : « Expédition brut »</span><span class="sxs-lookup"><span data-stu-id="6257d-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="6257d-257">à partir de : (« Sadie danield » ou « J’espère que brut »)</span><span class="sxs-lookup"><span data-stu-id="6257d-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="6257d-258">NOT</span><span class="sxs-lookup"><span data-stu-id="6257d-258">NOT</span></span>  <br/> |<span data-ttu-id="6257d-259">Non : « Ronnie Sturgis »</span><span class="sxs-lookup"><span data-stu-id="6257d-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="6257d-260">reçus : pas aujourd'hui</span><span class="sxs-lookup"><span data-stu-id="6257d-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="6257d-261">Notez que vous pouvez utiliser ces opérateurs pour joindre plusieurs critères ou pour joindre plusieurs valeurs dans une paire mot clé/valeur unique.</span><span class="sxs-lookup"><span data-stu-id="6257d-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="6257d-262">Cependant, pour prendre part à plusieurs valeurs dans une paire mot clé/valeur unique, vous devez utiliser entre parenthèses pour délimiter les valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="6257d-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="6257d-263">Pour comprendre pourquoi, envisagez de recherche à l’aide de : « Sadie Daniels » ou « Expédition brut ».</span><span class="sxs-lookup"><span data-stu-id="6257d-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="6257d-264">Cette recherche est interprétée comme les critères suivants :</span><span class="sxs-lookup"><span data-stu-id="6257d-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="6257d-265">L’élément provient Sadie danield, ou</span><span class="sxs-lookup"><span data-stu-id="6257d-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="6257d-266">L’élément a l’expression « Expédition brut » dans une de ses propriétés indexées.</span><span class="sxs-lookup"><span data-stu-id="6257d-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="6257d-267">En revanche, à partir de : (« Sadie Daniels » ou « Expédition brut ») est interprétée comme :</span><span class="sxs-lookup"><span data-stu-id="6257d-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="6257d-268">L’élément provient Sadie danield, ou</span><span class="sxs-lookup"><span data-stu-id="6257d-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="6257d-269">L’élément provient d’expédition brut</span><span class="sxs-lookup"><span data-stu-id="6257d-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="6257d-270">L’opérateur par défaut lorsque plusieurs critères sont spécifiés, mais aucun opérateur logique n’est inclus est and.</span><span class="sxs-lookup"><span data-stu-id="6257d-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="6257d-271">Par exemple, a des pièces jointes : true subject : projet équivaut à a : pièce jointe : true et subject : project.</span><span class="sxs-lookup"><span data-stu-id="6257d-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="6257d-272">Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6257d-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="6257d-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6257d-273"></span></span>

<span data-ttu-id="6257d-274">Dans cet exemple, une méthode appelée **SearchWithQueryString** est définie.</span><span class="sxs-lookup"><span data-stu-id="6257d-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="6257d-275">Il prend un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet de **type string** qui représente la chaîne de requête en tant que paramètres.</span><span class="sxs-lookup"><span data-stu-id="6257d-275">It takes an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="6257d-276">Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6257d-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

<span data-ttu-id="6257d-277">Vous pouvez utiliser cette méthode pour rechercher tous les éléments contenant l’expression « projet » dans l’objet, comme illustré dans cet exemple.</span><span class="sxs-lookup"><span data-stu-id="6257d-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="6257d-278">Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et les EWS</span><span class="sxs-lookup"><span data-stu-id="6257d-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="6257d-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="6257d-279"></span></span>

<span data-ttu-id="6257d-280">Dans cet exemple, une demande SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) recherche tous les éléments dans la boîte de réception avec l’expression « projet » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="6257d-280">In this example, a SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6257d-281">L’exemple suivant montre la réponse du serveur avec les résultats de recherche.</span><span class="sxs-lookup"><span data-stu-id="6257d-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6257d-282">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6257d-282">See also</span></span>

- [<span data-ttu-id="6257d-283">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6257d-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="6257d-284">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6257d-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="6257d-285">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="6257d-285">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="6257d-286">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="6257d-286">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

