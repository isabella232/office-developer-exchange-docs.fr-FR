---
title: Effectuer des recherches paginées à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre application EWS cible Exchange ou d’API managées.
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754922"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="ba688-103">Effectuer des recherches paginées à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba688-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="ba688-104">Découvrez comment effectuer des recherches paginées dans votre application EWS cible Exchange ou d’API managées.</span><span class="sxs-lookup"><span data-stu-id="ba688-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="ba688-105">Pagination est une fonctionnalité dans EWS qui vous permet de contrôler la taille des résultats d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="ba688-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="ba688-106">Au lieu d’extraire le jeu dans une réponse EWS de résultats, vous pouvez récupérer plus petits ensembles dans plusieurs réponses EWS.</span><span class="sxs-lookup"><span data-stu-id="ba688-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="ba688-107">Par exemple, imaginons un utilisateur disposant de 10 000 messages électroniques dans leur boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ba688-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="ba688-108">En théorie, vous pouvez récupérer tous les messages électroniques 10 000 dans une réponse de très grande taille, mais vous voudrez peut-être que diviser en segments plus facile à gérer pour des raisons de performances ou de la bande passante.</span><span class="sxs-lookup"><span data-stu-id="ba688-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="ba688-109">Pagination vous offre les outils à cette fin.</span><span class="sxs-lookup"><span data-stu-id="ba688-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ba688-110">Alors que vous pouvez récupérer théorie de 10 000 éléments dans une requête, en réalité, il s’agit probablement pas en raison de la limitation EWS.</span><span class="sxs-lookup"><span data-stu-id="ba688-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="ba688-111">Pour plus d’informations, voir [limitation EWS dans Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ba688-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="ba688-112">**Le tableau 1. Paramètres de pagination dans les API managées EWS**</span><span class="sxs-lookup"><span data-stu-id="ba688-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="ba688-113">**Pour configurer ou récupérer le...**</span><span class="sxs-lookup"><span data-stu-id="ba688-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="ba688-114">**Dans l’API managée EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="ba688-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="ba688-115">**Dans les services EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="ba688-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ba688-116">Nombre maximal d’éléments ou des dossiers dans une réponse</span><span class="sxs-lookup"><span data-stu-id="ba688-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="ba688-117">Le paramètre **pageSize** au [constructeur l’annonceAfficher](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) l’ou le [constructeur FolderView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-117">The **pageSize** parameter to the [ItemView constructor](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="ba688-118">Or</span><span class="sxs-lookup"><span data-stu-id="ba688-118">Or</span></span>  <br/> <span data-ttu-id="ba688-119">La propriété [PagedView.PageSize](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-119">The [PagedView.PageSize](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-120">L’attribut **MaxEntriesReturned** sur l’élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="ba688-121">Point de départ de la liste des éléments ou des dossiers</span><span class="sxs-lookup"><span data-stu-id="ba688-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="ba688-122">Le paramètre **offsetBasePoint** au constructeur **l’annonceAfficher** l’ou le constructeur **FolderView**</span><span class="sxs-lookup"><span data-stu-id="ba688-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="ba688-123">Or</span><span class="sxs-lookup"><span data-stu-id="ba688-123">Or</span></span>  <br/> <span data-ttu-id="ba688-124">La propriété [PagedView.OffsetBasePoint](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-124">The [PagedView.OffsetBasePoint](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-125">L’attribut de **point de base** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="ba688-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="ba688-126">Décalé du point de départ</span><span class="sxs-lookup"><span data-stu-id="ba688-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="ba688-127">Le paramètre **offset** au constructeur **l’annonceAfficher** l’ou le constructeur **FolderView**</span><span class="sxs-lookup"><span data-stu-id="ba688-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="ba688-128">Or</span><span class="sxs-lookup"><span data-stu-id="ba688-128">Or</span></span>  <br/> <span data-ttu-id="ba688-129">La propriété [PagedView.Offset](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-129">The [PagedView.Offset](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-130">L’attribut **Offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="ba688-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="ba688-131">Nombre total de résultats sur le serveur</span><span class="sxs-lookup"><span data-stu-id="ba688-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="ba688-132">La propriété [FindItemsResults.TotalCount](http://msdn.microsoft.com/fr-fr/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.TotalCount](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-132">The [FindItemsResults.TotalCount](http://msdn.microsoft.com/fr-fr/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-133">L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou l’élément [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="ba688-134">Décalage du premier élément ou un dossier non inclus dans la réponse en cours</span><span class="sxs-lookup"><span data-stu-id="ba688-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="ba688-135">La propriété [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/fr-fr/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-135">The [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/fr-fr/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-136">L’attribut **IndexedPagingOffset** sur l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="ba688-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="ba688-137">Indicateur que réponse inclut le dernier élément ou le dossier dans la liste</span><span class="sxs-lookup"><span data-stu-id="ba688-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="ba688-138">La propriété [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/fr-fr/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba688-138">The [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/fr-fr/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ba688-139">L’attribut **IncludesLastItemInRange** sur l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="ba688-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="ba688-140">Fonctionne de la pagination</span><span class="sxs-lookup"><span data-stu-id="ba688-140">How paging works</span></span>
<span data-ttu-id="ba688-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="ba688-141"></span></span>

<span data-ttu-id="ba688-142">Pour comprendre le fonctionne de la pagination, il est utile de visualiser les messages dans un dossier en tant que panneaux placés côte à côte dans un champ à l’extérieur de votre domicile.</span><span class="sxs-lookup"><span data-stu-id="ba688-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="ba688-143">Vous pouvez voir certains de ces panneaux d’affichage dans une fenêtre magique.</span><span class="sxs-lookup"><span data-stu-id="ba688-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="ba688-144">Vous avez la possibilité de modifier la taille de la fenêtre (pour voir plus ou moins de panneaux à la fois) et pour déplacer la fenêtre (pour contrôler les panneaux d’affichage que vous pouvez voir).</span><span class="sxs-lookup"><span data-stu-id="ba688-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="ba688-145">Cette manipulation de la fenêtre est la pagination.</span><span class="sxs-lookup"><span data-stu-id="ba688-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="ba688-146">Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="ba688-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="ba688-147">Vous définissez la position de la fenêtre en spécifiant un point de départ (le début de la ligne) ou la fin de la ligne et un décalage à partir de ce point de départ, exprimé en un nombre d’éléments.</span><span class="sxs-lookup"><span data-stu-id="ba688-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="ba688-148">Le début de la fenêtre est le nombre d’éléments spécifié par le décalage du point de départ.</span><span class="sxs-lookup"><span data-stu-id="ba688-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="ba688-149">Où pagination Obtient un peu plus intéressante est dans la réponse du serveur, et comment votre application peut utiliser la réponse à la requête suivante de la forme.</span><span class="sxs-lookup"><span data-stu-id="ba688-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="ba688-150">Le serveur fournit trois éléments d’information que vous pouvez utiliser pour déterminer comment configurer votre « fenêtre » pour votre requête suivante :</span><span class="sxs-lookup"><span data-stu-id="ba688-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="ba688-151">Si les résultats dans la réponse incluent le dernier élément dans le résultat global est défini sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ba688-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="ba688-152">Nombre total d’éléments dans le jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ba688-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="ba688-153">Ce que la valeur de décalage suivante doit être, si vous souhaitez passer la fenêtre à l’élément suivant dans le jeu de résultats qui n’est pas inclus dans la réponse en cours.</span><span class="sxs-lookup"><span data-stu-id="ba688-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="ba688-154">Voici un exemple simple.</span><span class="sxs-lookup"><span data-stu-id="ba688-154">Let's look at a simple example.</span></span> <span data-ttu-id="ba688-155">Imaginez une boîte de réception avec 15 messages.</span><span class="sxs-lookup"><span data-stu-id="ba688-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="ba688-156">Votre application envoie une demande initiale pour récupérer un maximum de 10 éléments, en commençant au début de la liste des messages (de sorte que le décalage est égale à zéro).</span><span class="sxs-lookup"><span data-stu-id="ba688-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="ba688-157">Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 10.</span><span class="sxs-lookup"><span data-stu-id="ba688-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="ba688-158">**La figure 1. Demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="ba688-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="ba688-160">Votre application puis renvoie la demande au serveur, avec le seul changement de même que le décalage est maintenant 10.</span><span class="sxs-lookup"><span data-stu-id="ba688-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="ba688-161">Le serveur renvoie les cinq derniers éléments et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 15 (bien évidemment, vous avez atteint la fin, il y un décalage suivant.)</span><span class="sxs-lookup"><span data-stu-id="ba688-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="ba688-162">**La figure 2. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="ba688-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="ba688-164">Considérations de conception pour la pagination</span><span class="sxs-lookup"><span data-stu-id="ba688-164">Design considerations for paging</span></span>
<span data-ttu-id="ba688-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="ba688-165"></span></span>

<span data-ttu-id="ba688-166">Tirer le meilleur parti pagination dans votre application nécessite en compte certains aspects.</span><span class="sxs-lookup"><span data-stu-id="ba688-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="ba688-167">Par exemple, la taille en faire votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="ba688-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="ba688-168">Que faire si les résultats sur le serveur modifiez alors que vous déplacez votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="ba688-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="ba688-169">Déterminer la taille de votre fenêtre</span><span class="sxs-lookup"><span data-stu-id="ba688-169">Determine the size of your window</span></span>

<span data-ttu-id="ba688-170">Il n’existe aucune « unique » nombre maximal d’entrées que toutes les applications doivent utiliser.</span><span class="sxs-lookup"><span data-stu-id="ba688-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="ba688-171">Détermination du nombre est un bon choix pour votre application dépend de plusieurs facteurs.</span><span class="sxs-lookup"><span data-stu-id="ba688-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="ba688-172">Toutefois, il est utile à garder à l’esprit les instructions suivantes :</span><span class="sxs-lookup"><span data-stu-id="ba688-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="ba688-173">Par défaut, Exchange limite le nombre maximal d’éléments pouvant être renvoyés dans une demande unique et 1000.</span><span class="sxs-lookup"><span data-stu-id="ba688-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="ba688-174">Si le nombre maximal d’entrées à une plus grande entraîne numéro que vous ayez à envoyer des demandes de moins pour obtenir tous les éléments, au détriment de devoir attendre plus de réponses.</span><span class="sxs-lookup"><span data-stu-id="ba688-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="ba688-175">Définir le nombre maximal d’entrées pour un plus petit nombre des résultats dans le temps de réponse plus rapides, au détriment de devoir envoyer plusieurs demandes pour obtenir tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="ba688-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="ba688-176">Gestion des modifications apportées au jeu de résultats</span><span class="sxs-lookup"><span data-stu-id="ba688-176">Handling changes to the result set</span></span>

<span data-ttu-id="ba688-177">Dans l’exemple simple plus haut dans cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur est resté constant.</span><span class="sxs-lookup"><span data-stu-id="ba688-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="ba688-178">Toutefois, en réalité, le nombre d’éléments dans une boîte de réception permettre changer fréquemment.</span><span class="sxs-lookup"><span data-stu-id="ba688-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="ba688-179">Nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment.</span><span class="sxs-lookup"><span data-stu-id="ba688-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="ba688-180">Mais comment cette pagination impact ?</span><span class="sxs-lookup"><span data-stu-id="ba688-180">But how does this impact paging?</span></span> <span data-ttu-id="ba688-181">Nous allons modifier l’exemple de scénario permettant de savoir antérieur.</span><span class="sxs-lookup"><span data-stu-id="ba688-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="ba688-182">Nous allons commencer à nouveau les 15 éléments dans la boîte de réception et envoyer la demande initiale de même.</span><span class="sxs-lookup"><span data-stu-id="ba688-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="ba688-183">Comme avant, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il n’y a un total de 15 éléments, et que le prochain offset doit être 10, comme le montre la Figure 1.</span><span class="sxs-lookup"><span data-stu-id="ba688-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="ba688-184">À présent, alors que votre application traite les 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté pour le jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ba688-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="ba688-185">Votre application renvoie la même requête sur le serveur (uniquement avec le décalage est défini sur 10).</span><span class="sxs-lookup"><span data-stu-id="ba688-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="ba688-186">Cette fois le serveur obtient en six éléments et indique qu’il n’y a un total de 16 éléments dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="ba688-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="ba688-187">À ce stade vous vous demandez peut-être si c’est même un problème.</span><span class="sxs-lookup"><span data-stu-id="ba688-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="ba688-188">Après tout, vous avez 16 éléments renvoyé sur les deux réponses, alors, pourquoi tous les tracas ?</span><span class="sxs-lookup"><span data-stu-id="ba688-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="ba688-189">La réponse dépend où le nouvel élément est placé dans la liste.</span><span class="sxs-lookup"><span data-stu-id="ba688-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="ba688-190">Si la liste est triée afin que les éléments les plus anciens (par date/heure de réception) sont d’abord, il n’existe aucun motif de préoccupation dans ce scénario.</span><span class="sxs-lookup"><span data-stu-id="ba688-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="ba688-191">Le nouvel élément sera passé à la fin de la liste et doivent être inclus dans la seconde réponse.</span><span class="sxs-lookup"><span data-stu-id="ba688-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="ba688-192">**La figure 3. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le 16e élément dans la liste en cours de nouveau**</span><span class="sxs-lookup"><span data-stu-id="ba688-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="ba688-194">Si la liste est triée afin que les éléments les plus récents sont d’abord, il est un autre article.</span><span class="sxs-lookup"><span data-stu-id="ba688-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="ba688-195">Dans ce cas, le premier élément de la deuxième demande serait le dernier élément de la requête précédente ainsi que les éléments restants cinq le 15 d’origine.</span><span class="sxs-lookup"><span data-stu-id="ba688-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="ba688-196">Pour mettre en termes de notre fenêtre magique imaginaire, vous déplacés de votre fenêtre par 10, mais les panneaux eux-mêmes sont également déplacés par 1.</span><span class="sxs-lookup"><span data-stu-id="ba688-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="ba688-197">**La figure 4. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le premier élément dans la liste en cours de nouveau**</span><span class="sxs-lookup"><span data-stu-id="ba688-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="ba688-199">Permet de détecter une modification dans les résultats sur le serveur consiste à utiliser le concept d’un élément d’ancrage.</span><span class="sxs-lookup"><span data-stu-id="ba688-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="ba688-200">Un élément d’ancrage est un élément supplémentaire dans votre réponse qui n’est pas traitée avec le reste des résultats, mais sert à comparer avec les résultats suivantes pour voir si les éléments ont déplacé.</span><span class="sxs-lookup"><span data-stu-id="ba688-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="ba688-201">Création de nouveau dans notre exemple, si votre application utilise une taille de « fenêtre » de 10, réellement définir le nombre maximal d’éléments à renvoyer à 11.</span><span class="sxs-lookup"><span data-stu-id="ba688-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="ba688-202">Votre application traite les 10 premiers éléments dans la réponse comme d’habitude.</span><span class="sxs-lookup"><span data-stu-id="ba688-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="ba688-203">Pour le dernier élément, enregistrez l’identificateur de l’élément comme point d’ancrage, puis publier la requête suivante avec un décalage de 10.</span><span class="sxs-lookup"><span data-stu-id="ba688-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="ba688-204">Si les données n’a pas changé, le premier élément de la deuxième réponse doit avoir un identificateur d’élément qui correspond à l’ancrage.</span><span class="sxs-lookup"><span data-stu-id="ba688-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="ba688-205">Si les identificateurs d’élément ne correspondent pas, vous savez que les données a été supprimées ou insérées dans les composants de la liste que vous avez déjà « paginée » sur.</span><span class="sxs-lookup"><span data-stu-id="ba688-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="ba688-206">Même lorsque vous savez que les données ont changé, vous devez toujours décider comment réagir.</span><span class="sxs-lookup"><span data-stu-id="ba688-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="ba688-207">Il n’existe pas soit une réponse unique pour cette question.</span><span class="sxs-lookup"><span data-stu-id="ba688-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="ba688-208">Vos actions dépend de la nature de votre application et elle est essentielle pour capturer tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="ba688-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="ba688-209">Vous pourrez ignorer complètement, redémarrez le processus à partir du début, ou sauvegarder le suivi et essayer de détecter où la modification a eu lieu.</span><span class="sxs-lookup"><span data-stu-id="ba688-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="ba688-210">Exemple : Effectuer une recherche paginée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ba688-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="ba688-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="ba688-211"></span></span>

<span data-ttu-id="ba688-212">Pagination est pris en charge par les méthodes API managées suivantes :</span><span class="sxs-lookup"><span data-stu-id="ba688-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="ba688-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-213">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="ba688-214">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-215">Folder.FindFolders</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-216">Folder.FindFolders</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="ba688-217">Si vous utilisez l’API managée EWS, votre application configure pagination avec la classe [l’annonceAfficher](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) l’ou [FolderView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit des informations à partir du serveur en ce qui concerne la pagination de la [FindItemsResults](http://msdn.microsoft.com/fr-fr/library/dd635381%28v=exchg.80%29.aspx) ou de [FindFoldersResults](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) classe.</span><span class="sxs-lookup"><span data-stu-id="ba688-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](http://msdn.microsoft.com/fr-fr/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="ba688-218">L’exemple suivant récupère tous les éléments dans un dossier à l’aide d’une recherche paginée qui renvoie les cinq éléments dans chaque réponse.</span><span class="sxs-lookup"><span data-stu-id="ba688-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="ba688-219">Elle récupère également un élément supplémentaire qui agira comme un point d’ancrage pour détecter les modifications apportées aux résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ba688-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="ba688-220">Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ba688-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems &amp;&amp; anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
            anchorId = results.Items.Last<Item>().Id;
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="ba688-221">Exemple : Effectuer une recherche paginée à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="ba688-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="ba688-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="ba688-222"></span></span>

<span data-ttu-id="ba688-223">Pagination est pris en charge par les opérations EWS suivantes :</span><span class="sxs-lookup"><span data-stu-id="ba688-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="ba688-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ba688-224">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="ba688-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="ba688-225">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="ba688-226">Si vous utilisez EWS, votre application configure pagination avec l’élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit des informations à partir du serveur en ce qui concerne la pagination de la [(RootFolder FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) élément ou l’élément [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ba688-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="ba688-227">Dans cet exemple de requête, une demande **FindItem** est envoyée pour un maximum de six éléments, en commençant à un offset de zéro depuis le début de la liste des éléments dans la boîte de réception de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba688-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ba688-228">Le serveur renvoie la réponse suivante, qui contient des éléments de six.</span><span class="sxs-lookup"><span data-stu-id="ba688-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="ba688-229">La réponse indique également qu’il n’y a un total de huit articles dans les résultats sur le serveur, et que le dernier élément dans la liste des résultats n’est pas présent dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="ba688-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="ba688-230">Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut de **décalage** est modifiée à cinq, ce qui indique que le serveur doit renvoyer au maximum six éléments en commençant au décalage de cinq à partir du début.</span><span class="sxs-lookup"><span data-stu-id="ba688-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ba688-231">Le serveur envoie la réponse suivante, qui contient trois éléments.</span><span class="sxs-lookup"><span data-stu-id="ba688-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="ba688-232">La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours huit et que le dernier élément dans les résultats de la liste est incluse dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="ba688-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ba688-233">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba688-233">See also</span></span>


- [<span data-ttu-id="ba688-234">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba688-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="ba688-235">Méthode ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-235">ExchangeService.FindFolders method</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-236">Méthode ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="ba688-236">ExchangeService.FindItems method</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-237">Méthode Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-237">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-238">Méthode Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="ba688-238">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ba688-239">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="ba688-239">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="ba688-240">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="ba688-240">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="ba688-241">Limitation EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba688-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

