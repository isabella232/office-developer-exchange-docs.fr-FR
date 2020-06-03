---
title: Effectuer une recherche AQS à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Découvrez comment effectuer des recherches à l’aide de chaînes de requête et de AQS dans votre application EWS ou API managée EWS.
localization_priority: Priority
ms.openlocfilehash: 9f611a8d90c6baf0f307897735c6366c82bb63c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455715"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="38253-103">Effectuer une recherche AQS à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38253-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="38253-104">Découvrez comment effectuer des recherches à l’aide de chaînes de requête et de AQS dans votre application EWS ou API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="38253-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="38253-105">Les chaînes de requête fournissent une alternative aux [filtres de recherche](how-to-use-search-filters-with-ews-in-exchange.md) pour exprimer des critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="38253-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="38253-106">Le plus grand avantage de l’utilisation des chaînes de requête est que vous n’êtes pas obligé de spécifier une seule propriété à rechercher.</span><span class="sxs-lookup"><span data-stu-id="38253-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="38253-107">Vous pouvez simplement indiquer une valeur, et la recherche s’appliquera à tous les champs couramment utilisés sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="38253-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="38253-108">Vous pouvez également affiner votre recherche à l’aide de la syntaxe de requête avancée (AQS) au lieu d’une valeur simple.</span><span class="sxs-lookup"><span data-stu-id="38253-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="38253-109">Toutefois, les chaînes de requête présentent les limitations suivantes que vous devez connaître avant de les ajouter à votre boîte à outils :</span><span class="sxs-lookup"><span data-stu-id="38253-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="38253-110">**La possibilité de rechercher des propriétés spécifiques est limitée.**</span><span class="sxs-lookup"><span data-stu-id="38253-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="38253-111">Lorsque vous effectuez une recherche avec une valeur simple dans une chaîne de requête, la recherche est effectuée sur toutes les propriétés indexées.</span><span class="sxs-lookup"><span data-stu-id="38253-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="38253-112">Vous pouvez affiner votre recherche à des propriétés spécifiques, mais les propriétés pouvant être utilisées dans une chaîne AQS sont limitées.</span><span class="sxs-lookup"><span data-stu-id="38253-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="38253-113">Si la propriété que vous souhaitez rechercher n’est pas l’une des propriétés disponibles pour AQS, envisagez d’utiliser un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="38253-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="38253-114">**Les propriétés personnalisées ne sont pas recherchées.**</span><span class="sxs-lookup"><span data-stu-id="38253-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="38253-115">Les recherches de chaîne de requête sont effectuées sur un index, et les propriétés personnalisées ne sont pas incluses dans cet index.</span><span class="sxs-lookup"><span data-stu-id="38253-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="38253-116">Si vous devez rechercher des propriétés personnalisées, utilisez plutôt un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="38253-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="38253-117">**Contrôle limité pour les recherches de chaînes.**</span><span class="sxs-lookup"><span data-stu-id="38253-117">**Limited control for string searches.**</span></span> <span data-ttu-id="38253-118">Les recherches de chaîne de requête ignorent toujours la casse, et sont toujours des recherches de sous-chaînes.</span><span class="sxs-lookup"><span data-stu-id="38253-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="38253-119">Si vous souhaitez effectuer des recherches en tenant compte de la casse, du préfixe ou de la correspondance exacte, utilisez un filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="38253-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="38253-120">**Non disponible pour les dossiers ou les dossiers de recherche.**</span><span class="sxs-lookup"><span data-stu-id="38253-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="38253-121">Les opérations EWS pour la recherche de dossiers ne prennent pas en charge l’utilisation d’une chaîne de requête.</span><span class="sxs-lookup"><span data-stu-id="38253-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="38253-122">En outre, les dossiers de recherche ne prennent pas en charge les chaînes de requête.</span><span class="sxs-lookup"><span data-stu-id="38253-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="38253-123">Dans les deux cas, un filtre de recherche est votre seule option.</span><span class="sxs-lookup"><span data-stu-id="38253-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="38253-124">Création d’une chaîne de requête</span><span class="sxs-lookup"><span data-stu-id="38253-124">Creating a query string</span></span>
<span data-ttu-id="38253-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="38253-125"><a name="bk_CreateQueryString"> </a></span></span>

<span data-ttu-id="38253-126">Les chaînes de requête dans l’API managée EWS et EWS sont interprétées comme un sous-ensemble de la syntaxe AQS.</span><span class="sxs-lookup"><span data-stu-id="38253-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="38253-127">Les chaînes AQS sont composées de valeurs ou de paires mot clé/valeur, séparées par un signe deux-points ( :).</span><span class="sxs-lookup"><span data-stu-id="38253-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="38253-128">Lorsqu’une valeur est spécifiée sans mot clé, toutes les propriétés indexées sont recherchées pour la valeur.</span><span class="sxs-lookup"><span data-stu-id="38253-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="38253-129">Si un mot clé est associé à une valeur, le mot clé spécifie une propriété à rechercher pour la valeur correspondante.</span><span class="sxs-lookup"><span data-stu-id="38253-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="38253-130">**Tableau 1. Mots clés AQS pris en charge**</span><span class="sxs-lookup"><span data-stu-id="38253-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="38253-131">**Mot clé**</span><span class="sxs-lookup"><span data-stu-id="38253-131">**Keyword**</span></span>|<span data-ttu-id="38253-132">**Type de valeur**</span><span class="sxs-lookup"><span data-stu-id="38253-132">**Value type**</span></span>|<span data-ttu-id="38253-133">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="38253-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38253-134">subject</span><span class="sxs-lookup"><span data-stu-id="38253-134">subject</span></span>  <br/> |<span data-ttu-id="38253-135">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-135">String</span></span>  <br/> |<span data-ttu-id="38253-136">Subject : Project</span><span class="sxs-lookup"><span data-stu-id="38253-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="38253-137">corps</span><span class="sxs-lookup"><span data-stu-id="38253-137">body</span></span>  <br/> |<span data-ttu-id="38253-138">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-138">String</span></span>  <br/> |<span data-ttu-id="38253-139">corps : chiffres de ventes</span><span class="sxs-lookup"><span data-stu-id="38253-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="38253-140">pièce jointe</span><span class="sxs-lookup"><span data-stu-id="38253-140">attachment</span></span>  <br/> |<span data-ttu-id="38253-141">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-141">String</span></span>  <br/> |<span data-ttu-id="38253-142">pièce jointe : rapport</span><span class="sxs-lookup"><span data-stu-id="38253-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="38253-143">au</span><span class="sxs-lookup"><span data-stu-id="38253-143">to</span></span>  <br/> |<span data-ttu-id="38253-144">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-144">String</span></span>  <br/> |<span data-ttu-id="38253-145">à : « Sadie Daniels »</span><span class="sxs-lookup"><span data-stu-id="38253-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="38253-146">from</span><span class="sxs-lookup"><span data-stu-id="38253-146">from</span></span>  <br/> |<span data-ttu-id="38253-147">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-147">String</span></span>  <br/> |<span data-ttu-id="38253-148">de : espérons</span><span class="sxs-lookup"><span data-stu-id="38253-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="38253-149">cc</span><span class="sxs-lookup"><span data-stu-id="38253-149">cc</span></span>  <br/> |<span data-ttu-id="38253-150">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-150">String</span></span>  <br/> |<span data-ttu-id="38253-151">CC : "Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="38253-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="38253-152">bcc</span><span class="sxs-lookup"><span data-stu-id="38253-152">bcc</span></span>  <br/> |<span data-ttu-id="38253-153">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-153">String</span></span>  <br/> |<span data-ttu-id="38253-154">CCI : Mack</span><span class="sxs-lookup"><span data-stu-id="38253-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="38253-155">participants</span><span class="sxs-lookup"><span data-stu-id="38253-155">participants</span></span>  <br/> |<span data-ttu-id="38253-156">Chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-156">String</span></span>  <br/> |<span data-ttu-id="38253-157">participants : Sadie</span><span class="sxs-lookup"><span data-stu-id="38253-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="38253-158">category</span><span class="sxs-lookup"><span data-stu-id="38253-158">category</span></span>  <br/> |<span data-ttu-id="38253-159">String</span><span class="sxs-lookup"><span data-stu-id="38253-159">String</span></span>  <br/> |<span data-ttu-id="38253-160">Catégorie : projet</span><span class="sxs-lookup"><span data-stu-id="38253-160">category:project</span></span>  <br/> |
|<span data-ttu-id="38253-161">importance</span><span class="sxs-lookup"><span data-stu-id="38253-161">importance</span></span>  <br/> |<span data-ttu-id="38253-162">String</span><span class="sxs-lookup"><span data-stu-id="38253-162">String</span></span>  <br/> |<span data-ttu-id="38253-163">importance:high</span><span class="sxs-lookup"><span data-stu-id="38253-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="38253-164">type</span><span class="sxs-lookup"><span data-stu-id="38253-164">kind</span></span>  <br/> |<span data-ttu-id="38253-165">Type d’élément</span><span class="sxs-lookup"><span data-stu-id="38253-165">Item type</span></span>  <br/> |<span data-ttu-id="38253-166">type : réunions</span><span class="sxs-lookup"><span data-stu-id="38253-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="38253-167">envoyé</span><span class="sxs-lookup"><span data-stu-id="38253-167">sent</span></span>  <br/> |<span data-ttu-id="38253-168">Date</span><span class="sxs-lookup"><span data-stu-id="38253-168">Date</span></span>  <br/> |<span data-ttu-id="38253-169">envoyés : 12/10/2013</span><span class="sxs-lookup"><span data-stu-id="38253-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="38253-170">reçu</span><span class="sxs-lookup"><span data-stu-id="38253-170">received</span></span>  <br/> |<span data-ttu-id="38253-171">Date</span><span class="sxs-lookup"><span data-stu-id="38253-171">Date</span></span>  <br/> |<span data-ttu-id="38253-172">reçu : hier</span><span class="sxs-lookup"><span data-stu-id="38253-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="38253-173">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="38253-173">hasattachment</span></span>  <br/> |<span data-ttu-id="38253-174">Valeur booléenne</span><span class="sxs-lookup"><span data-stu-id="38253-174">Boolean</span></span>  <br/> |<span data-ttu-id="38253-175">Avec pièce jointe : true</span><span class="sxs-lookup"><span data-stu-id="38253-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="38253-176">isflagged</span><span class="sxs-lookup"><span data-stu-id="38253-176">isflagged</span></span>  <br/> |<span data-ttu-id="38253-177">Valeur booléenne</span><span class="sxs-lookup"><span data-stu-id="38253-177">Boolean</span></span>  <br/> |<span data-ttu-id="38253-178">isflagged : true</span><span class="sxs-lookup"><span data-stu-id="38253-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="38253-179">IsRead</span><span class="sxs-lookup"><span data-stu-id="38253-179">isread</span></span>  <br/> |<span data-ttu-id="38253-180">Valeur booléenne</span><span class="sxs-lookup"><span data-stu-id="38253-180">Boolean</span></span>  <br/> |<span data-ttu-id="38253-181">IsRead : false</span><span class="sxs-lookup"><span data-stu-id="38253-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="38253-182">size</span><span class="sxs-lookup"><span data-stu-id="38253-182">size</span></span>  <br/> |<span data-ttu-id="38253-183">Nombre</span><span class="sxs-lookup"><span data-stu-id="38253-183">Number</span></span>  <br/> |<span data-ttu-id="38253-184">taille : \> 5000</span><span class="sxs-lookup"><span data-stu-id="38253-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="38253-185">Examinons le fonctionnement des différents types de valeur.</span><span class="sxs-lookup"><span data-stu-id="38253-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="38253-186">Utilisation d’un type de valeur de chaîne</span><span class="sxs-lookup"><span data-stu-id="38253-186">Using a string value type</span></span>

<span data-ttu-id="38253-187">Par défaut, les types de valeur de chaîne sont recherchés dans des recherches de sous-chaînes de préfixe qui ne respectent pas la casse.</span><span class="sxs-lookup"><span data-stu-id="38253-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="38253-188">Cela signifie que la recherche d’objet : Project correspond à l’un des objets suivants :</span><span class="sxs-lookup"><span data-stu-id="38253-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="38253-189">Notes de réunion Project</span><span class="sxs-lookup"><span data-stu-id="38253-189">Project meeting notes</span></span>
    
- <span data-ttu-id="38253-190">Avez-vous des plans de projet ?</span><span class="sxs-lookup"><span data-stu-id="38253-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="38253-191">Projections de ventes de décembre</span><span class="sxs-lookup"><span data-stu-id="38253-191">December sales projections</span></span>
    
<span data-ttu-id="38253-192">Vous pouvez modifier la recherche pour exiger le mot entier plutôt que les préfixes correspondants en encadrant la chaîne entre guillemets.</span><span class="sxs-lookup"><span data-stu-id="38253-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="38253-193">Recherche d’un objet : « projet » supprime la valeur « projections de ventes de décembre » de la liste des correspondances.</span><span class="sxs-lookup"><span data-stu-id="38253-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="38253-194">Notez que la valeur n’est toujours pas sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="38253-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="38253-195">Si vous utilisez plusieurs mots dans une chaîne de requête, une correspondance exige que les deux mots apparaissent dans les champs recherchés.</span><span class="sxs-lookup"><span data-stu-id="38253-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="38253-196">Par exemple, la recherche d’un objet : plan de projet correspond à l’un des objets suivants :</span><span class="sxs-lookup"><span data-stu-id="38253-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="38253-197">Plan de projet</span><span class="sxs-lookup"><span data-stu-id="38253-197">Project plan</span></span>
    
- <span data-ttu-id="38253-198">Avez-vous des plans de projet ?</span><span class="sxs-lookup"><span data-stu-id="38253-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="38253-199">Veuillez m’envoyer le plan de notre projet.</span><span class="sxs-lookup"><span data-stu-id="38253-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="38253-200">Planification des jalons du projet</span><span class="sxs-lookup"><span data-stu-id="38253-200">Planning project milestones</span></span>
    
<span data-ttu-id="38253-201">Si vous placez plusieurs mots entre guillemets, ils sont considérés comme une seule phrase.</span><span class="sxs-lookup"><span data-stu-id="38253-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="38253-202">Recherche d’un objet : « plan de projet » ne correspondait qu’au « plan de projet » de la liste précédente.</span><span class="sxs-lookup"><span data-stu-id="38253-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="38253-203">Utilisation d’un type de valeur de type d’élément</span><span class="sxs-lookup"><span data-stu-id="38253-203">Using an item type value type</span></span>

<span data-ttu-id="38253-204">Vous pouvez utiliser les valeurs de types d’éléments suivantes avec le mot clé **Kind** pour limiter les résultats de la recherche à un type d’élément spécifique, tel que les demandes de messagerie ou de réunion :</span><span class="sxs-lookup"><span data-stu-id="38253-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="38253-205">contacts</span><span class="sxs-lookup"><span data-stu-id="38253-205">contacts</span></span>    
- <span data-ttu-id="38253-206">docs</span><span class="sxs-lookup"><span data-stu-id="38253-206">docs</span></span>    
- <span data-ttu-id="38253-207">email</span><span class="sxs-lookup"><span data-stu-id="38253-207">email</span></span>    
- <span data-ttu-id="38253-208">faxes</span><span class="sxs-lookup"><span data-stu-id="38253-208">faxes</span></span>    
- <span data-ttu-id="38253-209">messagerie instantanée (correspond aux messages instantanés)</span><span class="sxs-lookup"><span data-stu-id="38253-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="38253-210">journals</span><span class="sxs-lookup"><span data-stu-id="38253-210">journals</span></span>    
- <span data-ttu-id="38253-211">réunions (correspond aux rendez-vous et aux demandes de réunion)</span><span class="sxs-lookup"><span data-stu-id="38253-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="38253-212">notes</span><span class="sxs-lookup"><span data-stu-id="38253-212">notes</span></span>    
- <span data-ttu-id="38253-213">posts</span><span class="sxs-lookup"><span data-stu-id="38253-213">posts</span></span>    
- <span data-ttu-id="38253-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="38253-214">rssfeeds</span></span>    
- <span data-ttu-id="38253-215">tasks</span><span class="sxs-lookup"><span data-stu-id="38253-215">tasks</span></span>    
- <span data-ttu-id="38253-216">voicemail</span><span class="sxs-lookup"><span data-stu-id="38253-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="38253-217">Utilisation d’un type de valeur de date</span><span class="sxs-lookup"><span data-stu-id="38253-217">Using a date value type</span></span>

<span data-ttu-id="38253-218">Vous pouvez rechercher des types de valeur de date de plusieurs façons différentes.</span><span class="sxs-lookup"><span data-stu-id="38253-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="38253-219">La plus simple consiste à rechercher une date spécifique.</span><span class="sxs-lookup"><span data-stu-id="38253-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="38253-220">Recherche avec reçus : 12/11/2013 renverra tous les éléments reçus le 11 décembre 2013.</span><span class="sxs-lookup"><span data-stu-id="38253-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="38253-221">Toutefois, vous pouvez également être moins spécifique.</span><span class="sxs-lookup"><span data-stu-id="38253-221">However, you can also be less specific.</span></span> <span data-ttu-id="38253-222">Recherche avec reçus : 12/11 renverra tous les éléments reçus le 11 décembre de l’année en cours.</span><span class="sxs-lookup"><span data-stu-id="38253-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="38253-223">Une autre option consiste à utiliser les noms de mois.</span><span class="sxs-lookup"><span data-stu-id="38253-223">Another option is to use the month names.</span></span> <span data-ttu-id="38253-224">Vous pouvez rechercher avec reçu le 11 décembre 2013 ou le 11 décembre pour obtenir les mêmes résultats que ceux reçus : 12/11/2013 et reçus : 12/11, respectivement.</span><span class="sxs-lookup"><span data-stu-id="38253-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="38253-225">Vous pouvez également effectuer une recherche avec received : décembre pour obtenir tous les éléments reçus dans le mois de décembre, dans l’année en cours.</span><span class="sxs-lookup"><span data-stu-id="38253-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="38253-226">L’utilisation des noms des jours de la semaine est également une option.</span><span class="sxs-lookup"><span data-stu-id="38253-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="38253-227">Recherche avec reçu : mardi renverra tous les éléments reçus le mardi de la semaine en cours.</span><span class="sxs-lookup"><span data-stu-id="38253-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="38253-228">Les types de valeur date prennent également en charge un ensemble de mots clés pour les recherches relatives à l’heure actuelle.</span><span class="sxs-lookup"><span data-stu-id="38253-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="38253-229">Les mots clés suivants sont pris en charge :</span><span class="sxs-lookup"><span data-stu-id="38253-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="38253-230">aujourd’hui</span><span class="sxs-lookup"><span data-stu-id="38253-230">today</span></span>  
- <span data-ttu-id="38253-231">demain</span><span class="sxs-lookup"><span data-stu-id="38253-231">tomorrow</span></span>
- <span data-ttu-id="38253-232">yesterday</span><span class="sxs-lookup"><span data-stu-id="38253-232">yesterday</span></span>
- <span data-ttu-id="38253-233">this week</span><span class="sxs-lookup"><span data-stu-id="38253-233">this week</span></span>    
- <span data-ttu-id="38253-234">La semaine dernière</span><span class="sxs-lookup"><span data-stu-id="38253-234">last week</span></span>    
- <span data-ttu-id="38253-235">mois suivant</span><span class="sxs-lookup"><span data-stu-id="38253-235">next month</span></span>    
- <span data-ttu-id="38253-236">mois précédent</span><span class="sxs-lookup"><span data-stu-id="38253-236">past month</span></span>    
- <span data-ttu-id="38253-237">année à venir</span><span class="sxs-lookup"><span data-stu-id="38253-237">coming year</span></span>
    
<span data-ttu-id="38253-238">Les types de valeur date peuvent également être comparés à des opérateurs relationnels comme supérieur ou inférieur à ou spécifiés en tant que plage avec l’opérateur de plage **..**. Par exemple, received : \> 11/30/2013, sent : \> = hier, et Received : 12/1/2013.. Today sont toutes des chaînes de requête valides.</span><span class="sxs-lookup"><span data-stu-id="38253-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="38253-239">Utilisation d’un type de valeur booléenne</span><span class="sxs-lookup"><span data-stu-id="38253-239">Using a Boolean value type</span></span>

<span data-ttu-id="38253-240">Les types de valeurs booléennes peuvent être « true » ou « false ».</span><span class="sxs-lookup"><span data-stu-id="38253-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="38253-241">Les valeurs ne respectent pas la casse, par conséquent IsRead : false produira les mêmes résultats que IsRead : FALSe.</span><span class="sxs-lookup"><span data-stu-id="38253-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="38253-242">Utilisation d’un type de valeur numérique</span><span class="sxs-lookup"><span data-stu-id="38253-242">Using a number value type</span></span>

<span data-ttu-id="38253-243">Les types de valeurs numériques peuvent être recherchés comme correspondances exactes, mais ils peuvent également faire l’objet d’une recherche à l’aide d’opérateurs relationnels comme supérieur ou inférieur à.</span><span class="sxs-lookup"><span data-stu-id="38253-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="38253-244">Par exemple, Size : 10000 renvoie uniquement les éléments dont la taille est égale à 10000 octets, mais Size : \> = 10000 renverra des éléments dont la taille est supérieure ou égale à 10000 octets.</span><span class="sxs-lookup"><span data-stu-id="38253-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="38253-245">Vous pouvez également spécifier une plage à l’aide de l’opérateur de plage ( **..**).</span><span class="sxs-lookup"><span data-stu-id="38253-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="38253-246">Par exemple, Size : 7000.. 8000 renverra des éléments dont la taille est comprise entre 7000 et 8000.</span><span class="sxs-lookup"><span data-stu-id="38253-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="38253-247">Utilisation d’opérateurs logiques</span><span class="sxs-lookup"><span data-stu-id="38253-247">Using logical operators</span></span>

<span data-ttu-id="38253-248">Les chaînes de requête prennent en charge les opérateurs logiques suivants.</span><span class="sxs-lookup"><span data-stu-id="38253-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="38253-249">**Tableau 2. Opérateurs logiques pris en charge**</span><span class="sxs-lookup"><span data-stu-id="38253-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="38253-250">**Opérateur**</span><span class="sxs-lookup"><span data-stu-id="38253-250">**Operator**</span></span>|<span data-ttu-id="38253-251">**Exemples**</span><span class="sxs-lookup"><span data-stu-id="38253-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38253-252">AND</span><span class="sxs-lookup"><span data-stu-id="38253-252">AND</span></span>  <br/> |<span data-ttu-id="38253-253">Project et from : "Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="38253-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="38253-254">objet : (Project et plan)</span><span class="sxs-lookup"><span data-stu-id="38253-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="38253-255">OR</span><span class="sxs-lookup"><span data-stu-id="38253-255">OR</span></span>  <br/> |<span data-ttu-id="38253-256">Subject : réunion ou de : « espoir brut »</span><span class="sxs-lookup"><span data-stu-id="38253-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="38253-257">from :("Sadie Daniels" ou "espoir brut")</span><span class="sxs-lookup"><span data-stu-id="38253-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="38253-258">NOT</span><span class="sxs-lookup"><span data-stu-id="38253-258">NOT</span></span>  <br/> |<span data-ttu-id="38253-259">NE provenant pas de : « Ronnie Sturgis »</span><span class="sxs-lookup"><span data-stu-id="38253-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="38253-260">reçu : pas aujourd’hui</span><span class="sxs-lookup"><span data-stu-id="38253-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="38253-261">Notez que vous pouvez utiliser ces opérateurs pour joindre plusieurs critères ou joindre plusieurs valeurs au sein d’une seule paire mot clé/valeur.</span><span class="sxs-lookup"><span data-stu-id="38253-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="38253-262">Toutefois, lorsque vous associez plusieurs valeurs dans une paire mot clé/valeur unique, vous devez utiliser des parenthèses pour encadrer les valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="38253-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="38253-263">Pour comprendre pourquoi, envisagez d’effectuer une recherche à partir de : « Sadie Daniels » ou « espérons brut ».</span><span class="sxs-lookup"><span data-stu-id="38253-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="38253-264">Cette recherche est en fait interprétée comme suit :</span><span class="sxs-lookup"><span data-stu-id="38253-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="38253-265">L’élément provient de Sadie Daniels ou</span><span class="sxs-lookup"><span data-stu-id="38253-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="38253-266">L’élément a l’expression « espoir brut » dans l’une de ses propriétés indexées.</span><span class="sxs-lookup"><span data-stu-id="38253-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="38253-267">En revanche, à partir de :(« Sadie Daniels » ou « espoir brut ») est interprétée comme :</span><span class="sxs-lookup"><span data-stu-id="38253-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="38253-268">L’élément provient de Sadie Daniels ou</span><span class="sxs-lookup"><span data-stu-id="38253-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="38253-269">L’article est d’espoir brut</span><span class="sxs-lookup"><span data-stu-id="38253-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="38253-270">Opérateur par défaut lorsque plusieurs critères sont spécifiés, mais qu’aucun opérateur logique n’est inclus, et.</span><span class="sxs-lookup"><span data-stu-id="38253-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="38253-271">Par exemple, comporte Attachment : true Subject : le projet équivaut à : Attachment : true et Subject : Project.</span><span class="sxs-lookup"><span data-stu-id="38253-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="38253-272">Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38253-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="38253-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="38253-273"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="38253-274">Dans cet exemple, une méthode appelée **SearchWithQueryString** est définie.</span><span class="sxs-lookup"><span data-stu-id="38253-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="38253-275">Il prend un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet **String** qui représente la chaîne de requête en tant que paramètres.</span><span class="sxs-lookup"><span data-stu-id="38253-275">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="38253-276">Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="38253-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

<span data-ttu-id="38253-277">Vous pouvez utiliser cette méthode pour rechercher tous les éléments avec l’expression « plan de projet » dans l’objet, comme illustré dans cet exemple.</span><span class="sxs-lookup"><span data-stu-id="38253-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="38253-278">Exemple : Rechercher des éléments à l’aide d’une chaîne de requête et EWS</span><span class="sxs-lookup"><span data-stu-id="38253-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="38253-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="38253-279"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="38253-280">Dans cet exemple, une requête [FINDITEM](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) SOAP recherche tous les éléments de la boîte de réception avec l’expression « plan Project » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="38253-280">In this example, a SOAP [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="38253-281">L’exemple suivant montre la réponse du serveur avec les résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="38253-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="38253-282">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38253-282">See also</span></span>

- [<span data-ttu-id="38253-283">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38253-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="38253-284">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38253-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="38253-285">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="38253-285">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="38253-286">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="38253-286">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

