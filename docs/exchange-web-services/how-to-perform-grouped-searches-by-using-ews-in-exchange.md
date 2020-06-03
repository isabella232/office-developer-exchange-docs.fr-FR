---
title: Effectuer des recherches groupées à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Découvrez comment effectuer des recherches groupées dans votre API managée EWS ou votre application EWS qui cible Exchange.
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527919"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a><span data-ttu-id="cf834-103">Effectuer des recherches groupées à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf834-103">Perform grouped searches by using EWS in Exchange</span></span>

<span data-ttu-id="cf834-104">Découvrez comment effectuer des recherches groupées dans votre API managée EWS ou votre application EWS qui cible Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf834-104">Find out how to perform grouped searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="cf834-105">Les recherches groupées sont utiles dans la mesure où elles vous permettent de contrôler la façon dont les résultats de la recherche sont organisés.</span><span class="sxs-lookup"><span data-stu-id="cf834-105">Grouped searches are useful in that they gives you control over how search results are organized.</span></span> <span data-ttu-id="cf834-106">Les résultats de la recherche organisés permettent à votre application de traiter plus facilement les résultats ou de les afficher à un utilisateur final de manière gérable.</span><span class="sxs-lookup"><span data-stu-id="cf834-106">Organized search results can make it easier for your application to process results or display them to an end user in a manageable way.</span></span>
  
<span data-ttu-id="cf834-107">Le regroupement consiste à placer tous les éléments dans le jeu de résultats qui ont la même valeur d’un champ spécifique dans un groupe.</span><span class="sxs-lookup"><span data-stu-id="cf834-107">Grouping works by putting all items within the result set that have the same value of a specific field into a group.</span></span> <span data-ttu-id="cf834-108">Par exemple, vous pouvez regrouper vos résultats par expéditeur et tous les éléments de la même personne se trouveront dans un groupe distinct, et les éléments de chaque groupe seront triés en fonction de l’ordre que vous spécifiez dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="cf834-108">For example, you can group your results by the sender, and all items from the same person will be in a separate group, and the items within each group will be sorted according to the order you specify on the view.</span></span> <span data-ttu-id="cf834-109">Les groupes eux-mêmes sont triés en fonction d’un champ que vous choisissez.</span><span class="sxs-lookup"><span data-stu-id="cf834-109">The groups themselves are sorted by an aggregate value based on a field you choose.</span></span>
  
<span data-ttu-id="cf834-110">**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour organiser les résultats de la recherche**</span><span class="sxs-lookup"><span data-stu-id="cf834-110">**Table 1. EWS Managed API methods and EWS operations for organizing search results**</span></span>

|<span data-ttu-id="cf834-111">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="cf834-111">**If you want to…**</span></span>|<span data-ttu-id="cf834-112">**Dans l’API managée EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="cf834-112">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="cf834-113">**Dans EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="cf834-113">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cf834-114">Organiser les éléments avec la même valeur dans une propriété spécifique de vos résultats dans des groupes</span><span class="sxs-lookup"><span data-stu-id="cf834-114">Organize items with the same value in a specific property in your results into groups</span></span>  <br/> |[<span data-ttu-id="cf834-115">GROUPING. Groupon</span><span class="sxs-lookup"><span data-stu-id="cf834-115">Grouping.GroupOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="cf834-116">Élément [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cf834-116">[FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="cf834-117">Trier les éléments de chaque groupe par valeur dans une propriété spécifique</span><span class="sxs-lookup"><span data-stu-id="cf834-117">Sort items within each group by the value in a specific property</span></span>  <br/> |[<span data-ttu-id="cf834-118">Objetitemview. OrderBy</span><span class="sxs-lookup"><span data-stu-id="cf834-118">ItemView.OrderBy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="cf834-119">[OrdreTri](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , élément</span><span class="sxs-lookup"><span data-stu-id="cf834-119">[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="cf834-120">Trier les groupes</span><span class="sxs-lookup"><span data-stu-id="cf834-120">Sort the groups</span></span>  <br/> |[<span data-ttu-id="cf834-121">GROUPING. AggregateOn</span><span class="sxs-lookup"><span data-stu-id="cf834-121">Grouping.AggregateOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="cf834-122">GROUPING. AggregateType</span><span class="sxs-lookup"><span data-stu-id="cf834-122">Grouping.AggregateType</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="cf834-123">GROUPING. SortDirection</span><span class="sxs-lookup"><span data-stu-id="cf834-123">Grouping.SortDirection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="cf834-124">Élément **FieldURI** en tant qu’enfant de l’élément [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cf834-124">**FieldURI** element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element</span></span><br/><br/> <span data-ttu-id="cf834-125">Attribut **Aggregate** sur l’élément **AggregateOn**</span><span class="sxs-lookup"><span data-stu-id="cf834-125">**Aggregate** attribute on the **AggregateOn** element</span></span><br/><br/><span data-ttu-id="cf834-126">Attribut **Order** sur l’élément **GroupBy**</span><span class="sxs-lookup"><span data-stu-id="cf834-126">**Order** attribute on the **GroupBy** element</span></span>  <br/> |
   
<span data-ttu-id="cf834-127">Nous allons procéder étape par étape.</span><span class="sxs-lookup"><span data-stu-id="cf834-127">Let's take it step by step.</span></span>
  
## <a name="group-results-by-a-specific-property"></a><span data-ttu-id="cf834-128">Regrouper les résultats par une propriété spécifique</span><span class="sxs-lookup"><span data-stu-id="cf834-128">Group results by a specific property</span></span>
<span data-ttu-id="cf834-129"><a name="bk_GroupResults"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-129"><a name="bk_GroupResults"> </a></span></span>

<span data-ttu-id="cf834-130">La première étape de l’utilisation du regroupement consiste à sélectionner une propriété, ou un attribut sur les éléments de la Banque d’aide Exchange, sur lequel effectuer le regroupement.</span><span class="sxs-lookup"><span data-stu-id="cf834-130">The first step to using grouping is to select a property, or attribute on the items in the Exchange store, to group by.</span></span> <span data-ttu-id="cf834-131">L’API managée EWS expose ces propriétés en tant que propriétés de classe sur les classes correspondantes, tandis que EWS les expose en tant qu’éléments XML.</span><span class="sxs-lookup"><span data-stu-id="cf834-131">The EWS Managed API exposes these as class properties on the corresponding classes, while EWS exposes them as XML elements.</span></span> <span data-ttu-id="cf834-132">Vous pouvez choisir n’importe quelle propriété, y compris des propriétés personnalisées ou étendues, mais il est utile de comprendre comment les éléments sont regroupés en fonction de la valeur de la propriété que vous choisissez.</span><span class="sxs-lookup"><span data-stu-id="cf834-132">You can choose any property, including custom or extended properties, but it is helpful to understand how items are grouped based on the value of the property you choose.</span></span> 

<span data-ttu-id="cf834-133">Tous les éléments qui ont la même valeur dans la propriété que vous choisissez de regrouper seront regroupés.</span><span class="sxs-lookup"><span data-stu-id="cf834-133">All items that have the same value in the property you choose to group by will be grouped together.</span></span> <span data-ttu-id="cf834-134">Cela peut sembler évident, mais il s’agit d’un détail important.</span><span class="sxs-lookup"><span data-stu-id="cf834-134">This might seem obvious, but it is an important detail.</span></span> <span data-ttu-id="cf834-135">Examinez ce qui se passe si vous regroupez par une propriété de date/heure, telle que [Item. DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) dans l’API managée EWS ou l’élément [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="cf834-135">Consider what happens if you group by a date/time property, such as [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) in the EWS Managed API, or the [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="cf834-136">L’objectif peut être d’organiser les résultats en groupes, chaque groupe contenant des éléments du même jour.</span><span class="sxs-lookup"><span data-stu-id="cf834-136">The intent might be to organize the results into groups, with each group containing items from the same day.</span></span> <span data-ttu-id="cf834-137">Toutefois, le regroupement examine l’ensemble de la valeur, ce qui inclut l’heure.</span><span class="sxs-lookup"><span data-stu-id="cf834-137">However, grouping looks at the entire value, which includes the time.</span></span> 

<span data-ttu-id="cf834-138">Le résultat final est que les éléments seront groupés de sorte que les éléments reçus en même temps, jusqu’au second, soient dans leurs propres groupes.</span><span class="sxs-lookup"><span data-stu-id="cf834-138">The end result is that the items will be grouped so that items received at the same time, down to the second, are in their own groups.</span></span> <span data-ttu-id="cf834-139">Les résultats seront probablement triés dans un grand nombre de groupes avec un petit nombre d’éléments dans chaque groupe.</span><span class="sxs-lookup"><span data-stu-id="cf834-139">The results will most likely be sorted into a large number of groups with a small number of items in each group.</span></span> 
  
<span data-ttu-id="cf834-140">Pour obtenir un jeu de résultats avec un plus petit nombre de groupes et un plus grand nombre d’éléments dans chaque groupe, choisissez une propriété susceptible de contenir un plus petit nombre de valeurs, telles que [EmailMessage. from](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) ou [Item. Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) dans l’API managée EWS, ou [à partir de ou de](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) [catégories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="cf834-140">To get a results set with a smaller number of groups and a larger number of items in each group, choose a property that is likely to have a smaller number of values, such as [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) or [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) in the EWS Managed API, or [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) or [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) in EWS.</span></span> <span data-ttu-id="cf834-141">La figure suivante montre une liste des courriers électroniques qui apparaissent dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="cf834-141">The following figure shows a list of emails that appear in an Inbox.</span></span> 
  
<span data-ttu-id="cf834-142">**Figure 1. Messages dans une boîte de réception**</span><span class="sxs-lookup"><span data-stu-id="cf834-142">**Figure 1. Messages in an Inbox**</span></span>

![Exemple de liste de messages dans la boîte de réception d’un utilisateur.](media/Ex15_GroupedSearch_MsgList.png)
  
<span data-ttu-id="cf834-144">Si vous regroupez les éléments de la figure 1 par la propriété **EmailMessage. from** , le résultat sera deux groupes, un pour les messages envoyés par l’espoir brut et un pour les messages envoyés par Sadie Daniels.</span><span class="sxs-lookup"><span data-stu-id="cf834-144">If you group the items in Figure 1 by the **EmailMessage.From** property, the result will be two groups, one for messages sent by Hope Gross, and one for messages sent by Sadie Daniels.</span></span> 
  
<span data-ttu-id="cf834-145">**Figure 2. Messages séparés en groupes en fonction de la propriété from**</span><span class="sxs-lookup"><span data-stu-id="cf834-145">**Figure 2. Messages separated into groups based on the From property**</span></span>

![Image affichant des messages triés dans deux listes par la propriété From.](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a><span data-ttu-id="cf834-147">Trier les éléments dans des groupes</span><span class="sxs-lookup"><span data-stu-id="cf834-147">Sort the items within groups</span></span>
<span data-ttu-id="cf834-148"><a name="bk_SortItems"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-148"><a name="bk_SortItems"> </a></span></span>

<span data-ttu-id="cf834-149">Vous pouvez contrôler la façon dont les éléments sont triés dans chaque groupe à l’aide de la propriété [objetitemview. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) de l’API managée EWS, ou de l’élément [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="cf834-149">You can control how items are sorted within each group by using the [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="cf834-150">Le même ordre s’applique à chaque groupe.</span><span class="sxs-lookup"><span data-stu-id="cf834-150">The same ordering applies to each group.</span></span> <span data-ttu-id="cf834-151">Par exemple, si vous triez les éléments de la figure 1 à l’aide de la propriété **Item. DateTimeReceived** , dans l’ordre décroissant, le dernier élément reçu d’espoir brut sera le premier dans le groupe brut de l’espoir, et le dernier élément reçu de Sadie Daniels sera d’abord dans le groupe Sadie Daniels.</span><span class="sxs-lookup"><span data-stu-id="cf834-151">For example, if you sort the items from Figure 1 by the **Item.DateTimeReceived** property, in descending order, the item most recently received from Hope Gross will be first in the Hope Gross group, and the item most recently received from Sadie Daniels will be first in the Sadie Daniels group.</span></span> <span data-ttu-id="cf834-152">De manière commode, les groupes de la figure 2 sont déjà triés de cette façon.</span><span class="sxs-lookup"><span data-stu-id="cf834-152">Conveniently, the groups in Figure 2 are already sorted this way.</span></span> 
  
## <a name="sort-the-groups"></a><span data-ttu-id="cf834-153">Trier les groupes</span><span class="sxs-lookup"><span data-stu-id="cf834-153">Sort the groups</span></span>
<span data-ttu-id="cf834-154"><a name="bk_SortGroups"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-154"><a name="bk_SortGroups"> </a></span></span>

<span data-ttu-id="cf834-155">À présent que vous avez réglé vos groupes, la dernière étape consiste à trier les groupes eux-mêmes.</span><span class="sxs-lookup"><span data-stu-id="cf834-155">Now that you have your groups settled, the final step is sorting the groups themselves.</span></span> <span data-ttu-id="cf834-156">Étant donné que les groupes eux-mêmes n’ont pas de valeurs spécifiques, le processus de regroupement doit affecter une valeur de tri à chaque groupe.</span><span class="sxs-lookup"><span data-stu-id="cf834-156">Because the groups themselves have no specific values, the grouping process has to assign a sort value to each group.</span></span> <span data-ttu-id="cf834-157">Cette opération est réalisée par agrégation des valeurs d’une propriété spécifique au sein de chaque groupe, spécifiée par la propriété [Grouping. AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) dans l’API managée EWS ou l’élément [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) en tant qu’enfant de l’élément [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="cf834-157">This is done by aggregation of the values of a specific property within each group, specified by the [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="cf834-158">La propriété [Grouping. AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) de l’API managée EWS (ou l’attribut **Aggregate** sur l’élément **AggregateOn** dans EWS) spécifie quelle valeur des éléments de chaque groupe est affectée à la valeur de tri du groupe, soit la plus grande valeur, soit la plus petite.</span><span class="sxs-lookup"><span data-stu-id="cf834-158">The [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) property in the EWS Managed API (or the **Aggregate** attribute on the **AggregateOn** element in EWS) specifies which value from the items within each group is assigned to the sort value for the group — either the largest value or the smallest value.</span></span> <span data-ttu-id="cf834-159">Enfin, l’ordre de tri (décroissant ou croissant) est spécifié par la propriété [Grouping. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) de l’API managée EWS ou l’attribut **Order** de l’élément [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) dans EWS.</span><span class="sxs-lookup"><span data-stu-id="cf834-159">Finally, the sort order (descending or ascending) is specified by the [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) property in the EWS Managed API, or the **Order** attribute on the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="cf834-160">Par exemple, si les groupes de la figure 2 sont triés par agrégation sur la propriété **Item. DateTimeReceived** , en utilisant la plus petite valeur et un tri par ordre décroissant, les éléments sont renvoyés dans l’ordre indiqué dans la figure 3.</span><span class="sxs-lookup"><span data-stu-id="cf834-160">For example, if the groups from Figure 2 are sorted by aggregating on the **Item.DateTimeReceived** property, using the smallest value, and sorting in descending order, the items are returned in the order in shown Figure 3.</span></span> 
  
<span data-ttu-id="cf834-161">**Figure 3. Résultats de recherche groupés avec les groupes triés par la propriété DateTimeReceived**</span><span class="sxs-lookup"><span data-stu-id="cf834-161">**Figure 3. Grouped search results with the groups sorted by the DateTimeReceived property**</span></span>

![Image montrant une liste triée de messages, regroupés par la propriété From, avec les groupes triés en fonction de la date/heure de réception la plus récente.](media/Ex15_GroupedSearch_Results.png)
  
<span data-ttu-id="cf834-163">Les sections suivantes montrent comment vous pouvez extraire ensemble le regroupement et le tri dans le code.</span><span class="sxs-lookup"><span data-stu-id="cf834-163">The next sections show you how you might pull grouping and sorting together in code.</span></span>
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a><span data-ttu-id="cf834-164">Exemple : effectuer une recherche groupée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="cf834-164">Example: Perform a grouped search by using the EWS Managed API</span></span>
<span data-ttu-id="cf834-165"><a name="bk_GroupSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-165"><a name="bk_GroupSearchEWSMA"> </a></span></span>

<span data-ttu-id="cf834-166">Les méthodes d’API managée EWS suivantes peuvent utiliser le regroupement :</span><span class="sxs-lookup"><span data-stu-id="cf834-166">The following EWS Managed API methods can use grouping:</span></span>
  
- [<span data-ttu-id="cf834-167">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="cf834-167">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cf834-168">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="cf834-168">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="cf834-169">L’exemple suivant utilise la méthode **ExchangeService. FindItems** ; Toutefois, les mêmes règles et concepts s’appliquent à la méthode **Folder. FindItems** .</span><span class="sxs-lookup"><span data-stu-id="cf834-169">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to the **Folder.FindItems** method.</span></span> <span data-ttu-id="cf834-170">Dans cet exemple, une méthode appelée **GroupItemsByFrom** est définie.</span><span class="sxs-lookup"><span data-stu-id="cf834-170">In this example, a method called **GroupItemsByFrom** is defined.</span></span> <span data-ttu-id="cf834-171">Il utilise un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et un objet [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) comme paramètres.</span><span class="sxs-lookup"><span data-stu-id="cf834-171">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="cf834-172">Il demande les premiers 50 éléments du dossier, groupés par la propriété **EmailMessage. from** , triée par la propriété **Item. DateTimeReceived** dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="cf834-172">It requests the first 50 items in the folder, grouped by the **EmailMessage.From** property, sorted by the **Item.DateTimeReceived** property in descending order.</span></span> <span data-ttu-id="cf834-173">Les groupes sont triés par valeur de propriété **Item. DateTimeReceived** sur leurs éléments, par ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="cf834-173">The groups themselves are sorted by the smallest **Item.DateTimeReceived** property value on their items, in descending order.</span></span> 
  
<span data-ttu-id="cf834-174">Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="cf834-174">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a><span data-ttu-id="cf834-175">Exemple : effectuer une recherche groupée à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="cf834-175">Example: Perform a grouped search by using EWS</span></span>
<span data-ttu-id="cf834-176"><a name="bk_GroupSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-176"><a name="bk_GroupSearchEWS"> </a></span></span>

<span data-ttu-id="cf834-177">L’exemple de requête suivant montre une demande d' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour les premiers éléments 50 dans le dossier, regroupés par l’élément **from** , trié par l’élément **DateTimeReceived** dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="cf834-177">The following request example shows a [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request for the first 50 items in the folder, grouped by the **From** element, sorted by the **DateTimeReceived** element in descending order.</span></span> <span data-ttu-id="cf834-178">Les groupes sont triés en fonction de la plus petite valeur de l’élément **DateTimeReceived** sur leurs éléments, dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="cf834-178">The groups themselves are sorted by the smallest **DateTimeReceived** element value on their items, in descending order.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
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

<span data-ttu-id="cf834-179">Le serveur renvoie la réponse suivante.</span><span class="sxs-lookup"><span data-stu-id="cf834-179">The server returns the following response.</span></span>
  
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
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="cf834-180">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="cf834-180">Version differences</span></span>
<span data-ttu-id="cf834-181"><a name="bk_VersionDiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="cf834-181"><a name="bk_VersionDiffs"> </a></span></span>

<span data-ttu-id="cf834-182">Les versions d’Exchange commençant par la version principale 15 et se terminant par Build 15.0.775.38 renvoient les éléments de **groupe** (de type **GroupedItemsType**) à la place des éléments [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) dans la réponse SOAP.</span><span class="sxs-lookup"><span data-stu-id="cf834-182">Versions of Exchange starting with major version 15 and ending with build 15.0.775.38 return **Group** elements (of type **GroupedItemsType**) in place of [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) elements in the SOAP response.</span></span> <span data-ttu-id="cf834-183">Si vous utilisez l’API managée EWS, la collection [GroupedFindItemsResults. ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) doit contenir 0 objet.</span><span class="sxs-lookup"><span data-stu-id="cf834-183">If you are using the EWS Managed API, this will cause the [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) collection to contain 0 objects.</span></span> <span data-ttu-id="cf834-184">Si vous utilisez EWS, les éléments de **groupe** doivent être traités comme des éléments **GroupedItems** .</span><span class="sxs-lookup"><span data-stu-id="cf834-184">If you are using EWS, **Group** elements should be handled as **GroupedItems** elements.</span></span> 
  
<span data-ttu-id="cf834-185">Les versions d’Exchange commençant par la version principale 15 renvoient des éléments **Group** ou **GroupedItems** avec l’attribut **xsi : Nil** défini sur **true** dans la réponse SOAP.</span><span class="sxs-lookup"><span data-stu-id="cf834-185">Versions of Exchange starting with major version 15 return extra **Group** or **GroupedItems** elements with the **xsi:nil** attribute set to **true** in the SOAP response.</span></span> <span data-ttu-id="cf834-186">Si vous utilisez l’API managée EWS, ces éléments supplémentaires entraînent la levée d’une [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="cf834-186">If you are using the EWS Managed API, these extra elements will cause a [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) to be thrown.</span></span> <span data-ttu-id="cf834-187">Si vous utilisez EWS, ces éléments supplémentaires doivent être ignorés.</span><span class="sxs-lookup"><span data-stu-id="cf834-187">If you are using EWS, these extra elements should be ignored.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cf834-188">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf834-188">See also</span></span>

- [<span data-ttu-id="cf834-189">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf834-189">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="cf834-190">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="cf834-190">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="cf834-191">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="cf834-191">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="cf834-192">Classe GROUPING</span><span class="sxs-lookup"><span data-stu-id="cf834-192">Grouping class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="cf834-193">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="cf834-193">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

