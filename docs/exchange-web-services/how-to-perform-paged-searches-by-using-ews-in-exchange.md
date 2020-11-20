---
title: Effectuer des recherches paginées à l’aide des services web Exchange (EWS) dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre API gérée EWS ou votre application EWS qui cible Exchange.
localization_priority: Priority
ms.openlocfilehash: fa36a2ce77150f29e5a62876138c9693a3b4ab1f
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348821"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="cd143-103">Effectuer des recherches paginées à l’aide des services web Exchange (EWS) dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cd143-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="cd143-104">Découvrez comment effectuer des recherches paginées dans votre API gérée EWS ou votre application EWS qui cible Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd143-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="cd143-105">La pagination est une fonctionnalité de EWS qui vous permet de contrôler la taille des résultats d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="cd143-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="cd143-106">Plutôt que de récupérer l’ensemble de résultats dans une seule réponse EWS, vous pouvez récupérer des ensembles plus petits dans plusieurs réponses EWS.</span><span class="sxs-lookup"><span data-stu-id="cd143-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="cd143-107">Par exemple, prenons un utilisateur avec 10 000 e-mails dans sa boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="cd143-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="cd143-108">En théorie, vous pouvez récupérer les 10 000 e-mails en une seule réponse très volumineuse, mais vous voudrez peut-être diviser ces données en blocs plus gérables pour des raisons de bande passante ou de performances.</span><span class="sxs-lookup"><span data-stu-id="cd143-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="cd143-109">La pagination vous donne les outils pour effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="cd143-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="cd143-110">Bien que vous puissiez, en théorie, récupérer 10 000 éléments en une seule requête, cela est peu probable en réalité en raison de la limitation EWS.</span><span class="sxs-lookup"><span data-stu-id="cd143-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="cd143-111">Si vous souhaitez en savoir plus, consultez l’article [Limitation EWS dans Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cd143-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="cd143-112">**Tableau 1. Paramètres de pagination dans l’API gérée EWS et EWS**</span><span class="sxs-lookup"><span data-stu-id="cd143-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="cd143-113">**Pour configurer ou récupérer…**</span><span class="sxs-lookup"><span data-stu-id="cd143-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="cd143-114">**Dans l’API gérée EWS, utilisez…**</span><span class="sxs-lookup"><span data-stu-id="cd143-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="cd143-115">**Dans EWS, utilisez…**</span><span class="sxs-lookup"><span data-stu-id="cd143-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cd143-116">Le nombre maximum d’éléments ou de dossiers dans une réponse</span><span class="sxs-lookup"><span data-stu-id="cd143-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="cd143-117">Le paramètre **pageSize** du [constructeur ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou du [constructeur FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="cd143-118">Ou</span><span class="sxs-lookup"><span data-stu-id="cd143-118">Or</span></span>  <br/> <span data-ttu-id="cd143-119">La propriété [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-120">L’attribut **MaxEntriesReturned** de l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou de l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="cd143-121">Le point de départ dans la liste des éléments ou des dossiers</span><span class="sxs-lookup"><span data-stu-id="cd143-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="cd143-122">Le paramètre **offsetBasePoint** du constructeur **ItemView** ou du constructeur **FolderView** </span><span class="sxs-lookup"><span data-stu-id="cd143-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="cd143-123">Ou</span><span class="sxs-lookup"><span data-stu-id="cd143-123">Or</span></span>  <br/> <span data-ttu-id="cd143-124">La propriété [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-125">L’attribut **BasePoint** de l’élément **IndexedPageItemView** ou de l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="cd143-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="cd143-126">Le décalage par rapport au point de départ</span><span class="sxs-lookup"><span data-stu-id="cd143-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="cd143-127">Le paramètre **offset** du constructeur **ItemView** ou du constructeur **FolderView**</span><span class="sxs-lookup"><span data-stu-id="cd143-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="cd143-128">Ou</span><span class="sxs-lookup"><span data-stu-id="cd143-128">Or</span></span>  <br/> <span data-ttu-id="cd143-129">La propriété [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-130">L’attribut **Offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="cd143-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="cd143-131">Le nombre total de résultats sur le serveur</span><span class="sxs-lookup"><span data-stu-id="cd143-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="cd143-132">La propriété [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-133">L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou sur l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="cd143-134">Le décalage du premier élément ou dossier non inclus dans la réponse actuelle</span><span class="sxs-lookup"><span data-stu-id="cd143-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="cd143-135">La [propriété FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-136">L’attribut **IndexedPagingOffset** sur l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="cd143-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="cd143-137">L’indicateur indiquant que la réponse inclut le dernier élément ou dossier de la liste</span><span class="sxs-lookup"><span data-stu-id="cd143-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="cd143-138">La propriété [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="cd143-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="cd143-139">L’attribut **includesLastItemInRange** sur l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="cd143-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="cd143-140">Fonctionnement de la pagination</span><span class="sxs-lookup"><span data-stu-id="cd143-140">How paging works</span></span>
<span data-ttu-id="cd143-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="cd143-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="cd143-142">Pour comprendre le fonctionnement de la pagination, imaginez les messages dans un dossier comme des panneaux d’affichage alignés côte à côte dans un champ à l’extérieur de votre maison.</span><span class="sxs-lookup"><span data-stu-id="cd143-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="cd143-143">Vous pouvez voir certains de ces panneaux à travers une fenêtre magique.</span><span class="sxs-lookup"><span data-stu-id="cd143-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="cd143-144">Vous avez la possibilité de modifier la taille de la fenêtre (pour voir plus ou moins de panneaux d’affichage à la fois) et de déplacer la fenêtre (pour contrôler les panneaux d’affichage que vous pouvez voir).</span><span class="sxs-lookup"><span data-stu-id="cd143-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="cd143-145">Cette manipulation de la fenêtre est une pagination.</span><span class="sxs-lookup"><span data-stu-id="cd143-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="cd143-146">Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="cd143-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="cd143-147">Vous définissez la position de la fenêtre en spécifiant un point de départ (soit le début de la ligne, soit la fin de la ligne) et un décalage par rapport à ce point de départ, exprimé en nombre d’éléments.</span><span class="sxs-lookup"><span data-stu-id="cd143-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="cd143-148">Le début de la fenêtre correspond au nombre d’éléments spécifié par le décalage par rapport au point de départ.</span><span class="sxs-lookup"><span data-stu-id="cd143-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="cd143-149">Là où la pagination devient un peu plus intéressante, c’est dans la réponse du serveur et dans la manière dont votre application peut utiliser cette réponse pour façonner sa prochaine requête.</span><span class="sxs-lookup"><span data-stu-id="cd143-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="cd143-150">Le serveur vous donne trois informations que vous pouvez utiliser pour déterminer comment configurer votre « fenêtre » pour votre prochaine requête :</span><span class="sxs-lookup"><span data-stu-id="cd143-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="cd143-151">Indique si les résultats de la réponse incluent le dernier élément de l’ensemble de résultats global sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="cd143-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="cd143-152">Le nombre total d’éléments dans le jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="cd143-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="cd143-153">Quelle devrait être la valeur de décalage suivante, si vous souhaitez faire avancer votre fenêtre vers l’élément suivant du jeu de résultats qui n’est pas inclus dans la réponse actuelle.</span><span class="sxs-lookup"><span data-stu-id="cd143-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="cd143-154">Prenons un exemple simple.</span><span class="sxs-lookup"><span data-stu-id="cd143-154">Let's look at a simple example.</span></span> <span data-ttu-id="cd143-155">Imaginez une boîte de réception contenant 15 messages.</span><span class="sxs-lookup"><span data-stu-id="cd143-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="cd143-156">Votre application envoie une demande initiale pour récupérer un maximum de 10 éléments, en commençant au début de la liste des messages (le décalage est donc nul).</span><span class="sxs-lookup"><span data-stu-id="cd143-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="cd143-157">Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments et que le décalage suivant doit être de 10.</span><span class="sxs-lookup"><span data-stu-id="cd143-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="cd143-158">**Figure 1. Demande de 10 éléments avec un décalage de 0 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="cd143-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="cd143-160">Votre application renvoie ensuite la même demande au serveur, le seul changement étant que le décalage est désormais de 10.</span><span class="sxs-lookup"><span data-stu-id="cd143-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="cd143-161">Le serveur renvoie les cinq derniers éléments et indique que la réponse inclut le dernier élément, qu’il y a un total de 15 éléments et que le prochain décalage devrait être de 15 (même si vous avez atteint la fin de la liste et qu’il n’y aura pas de prochain décalage).</span><span class="sxs-lookup"><span data-stu-id="cd143-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="cd143-162">**Figure 2. Demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="cd143-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="cd143-164">Aspects de conception à prendre en compte pour la pagination</span><span class="sxs-lookup"><span data-stu-id="cd143-164">Design considerations for paging</span></span>
<span data-ttu-id="cd143-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="cd143-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="cd143-166">Profiter du meilleur de la pagination dans votre application nécessite une certaine réflexion.</span><span class="sxs-lookup"><span data-stu-id="cd143-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="cd143-167">Par exemple, quelle est la taille de votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="cd143-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="cd143-168">Que faites-vous si les résultats sur le serveur changent pendant que vous déplacez votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="cd143-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="cd143-169">Déterminer la taille de votre fenêtre</span><span class="sxs-lookup"><span data-stu-id="cd143-169">Determine the size of your window</span></span>

<span data-ttu-id="cd143-170">Il n’y a pas de nombre maximum d’entrées à « taille unique » que toutes les applications doivent utiliser.</span><span class="sxs-lookup"><span data-stu-id="cd143-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="cd143-171">Déterminer le nombre qui convient à votre application dépend de plusieurs facteurs différents.</span><span class="sxs-lookup"><span data-stu-id="cd143-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="cd143-172">Cependant, il est utile de garder à l’esprit les instructions suivantes :</span><span class="sxs-lookup"><span data-stu-id="cd143-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="cd143-173">Par défaut, Exchange limite le nombre maximal d’éléments pouvant être retournés dans une seule demande à 1 000.</span><span class="sxs-lookup"><span data-stu-id="cd143-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="cd143-174">Si vous définissez le nombre maximum d’entrées sur un nombre plus élevé, vous devez envoyer moins de demandes pour obtenir tous les éléments, mais vous devrez attendre plus longtemps pour obtenir les réponses.</span><span class="sxs-lookup"><span data-stu-id="cd143-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="cd143-175">Si vous définissez le nombre maximum d’entrées sur un nombre plus petit, les réponses sont plus rapides, mais vous devrez envoyer plus de demandes pour obtenir tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="cd143-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="cd143-176">Gérer les modifications du jeu de résultats</span><span class="sxs-lookup"><span data-stu-id="cd143-176">Handling changes to the result set</span></span>

<span data-ttu-id="cd143-177">Dans l’exemple simple présenté au début de cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur est resté constant.</span><span class="sxs-lookup"><span data-stu-id="cd143-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="cd143-178">Toutefois, dans la réalité, le nombre d’éléments dans une boîte de réception peut changer fréquemment.</span><span class="sxs-lookup"><span data-stu-id="cd143-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="cd143-179">De nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment.</span><span class="sxs-lookup"><span data-stu-id="cd143-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="cd143-180">En quoi cela affecte-t-il la pagination ?</span><span class="sxs-lookup"><span data-stu-id="cd143-180">But how does this impact paging?</span></span> <span data-ttu-id="cd143-181">Nous allons modifier l’exemple de scénario précédent pour le découvrir.</span><span class="sxs-lookup"><span data-stu-id="cd143-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="cd143-182">Nous allons recommencer avec les 15 éléments de la boîte de réception de l’utilisateur et allons envoyer la même demande initiale.</span><span class="sxs-lookup"><span data-stu-id="cd143-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="cd143-183">Comme dans l’exemple précédent, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments et que le décalage suivant doit être de 10, comme le montre la figure 1.</span><span class="sxs-lookup"><span data-stu-id="cd143-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="cd143-184">Mais, pendant que votre application traite ces 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté au jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="cd143-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="cd143-185">Votre application renvoie la même demande au serveur (uniquement avec le décalage défini sur 10).</span><span class="sxs-lookup"><span data-stu-id="cd143-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="cd143-186">Cette fois, le serveur récupère six éléments et indique qu’il y a un total de 16 éléments dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="cd143-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="cd143-187">À ce stade, vous vous demandez peut-être en quoi cela est un problème.</span><span class="sxs-lookup"><span data-stu-id="cd143-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="cd143-188">Après tout, vous avez récupéré 16 éléments sur les deux réponses, alors pourquoi s’en faire ?</span><span class="sxs-lookup"><span data-stu-id="cd143-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="cd143-189">La réponse dépend du placement du nouvel élément dans la liste.</span><span class="sxs-lookup"><span data-stu-id="cd143-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="cd143-190">Si la liste est triée de manière à ce que les éléments les plus anciens (par date ou heure de réception) soient les premiers, il n’y a pas lieu de s’inquiéter dans ce scénario.</span><span class="sxs-lookup"><span data-stu-id="cd143-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="cd143-191">Le nouvel élément sera placé à la fin de la liste et sera inclus dans la deuxième réponse.</span><span class="sxs-lookup"><span data-stu-id="cd143-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="cd143-192">**Figure 3. Demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments, le 16e élément de la liste étant nouveau**</span><span class="sxs-lookup"><span data-stu-id="cd143-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="cd143-194">Si la liste est triée de manière à ce que les éléments les plus récents soient les premiers, c’est une autre histoire.</span><span class="sxs-lookup"><span data-stu-id="cd143-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="cd143-195">Dans ce cas, le premier élément de la deuxième demande serait le dernier élément de la demande précédente en plus des cinq éléments restants des 15 éléments d’origine.</span><span class="sxs-lookup"><span data-stu-id="cd143-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="cd143-196">Pour reprendre l’image de notre fenêtre magique imaginaire, vous avez déplacé la position de votre fenêtre de 10, mais les panneaux d’affichage eux-mêmes ont également été décalés de 1.</span><span class="sxs-lookup"><span data-stu-id="cd143-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="cd143-197">**Figure 4. Demande de 10 éléments avec un décalage de 10 depuis le début d’une liste de 16 éléments, le premier élément de la liste étant nouveau**</span><span class="sxs-lookup"><span data-stu-id="cd143-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments avec un décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="cd143-199">Une façon de détecter une modification des résultats sur le serveur consiste à utiliser le concept d’élément d’ancrage.</span><span class="sxs-lookup"><span data-stu-id="cd143-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="cd143-200">Un élément d’ancrage est un élément supplémentaire dans votre réponse qui n’est pas traité avec le reste des résultats, mais est utilisé pour effectuer une comparaison avec les résultats suivants pour voir si les éléments eux-mêmes ont changé.</span><span class="sxs-lookup"><span data-stu-id="cd143-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="cd143-201">En se basant à nouveau sur notre exemple simple, si votre application utilise une taille de « fenêtre » de 10, vous définissez en fait le nombre maximum d’éléments à retourner sur 11.</span><span class="sxs-lookup"><span data-stu-id="cd143-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="cd143-202">Votre application traite les 10 premiers éléments de la réponse comme d’habitude.</span><span class="sxs-lookup"><span data-stu-id="cd143-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="cd143-203">Pour le dernier élément, vous enregistrez l’identifiant de l’élément en tant qu’ancre, puis émettez la demande suivante avec un décalage de 10.</span><span class="sxs-lookup"><span data-stu-id="cd143-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="cd143-204">Si les données n’ont pas changé, le premier élément de la deuxième réponse doit avoir un identifiant d’élément qui correspond à l’ancre.</span><span class="sxs-lookup"><span data-stu-id="cd143-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="cd143-205">Si les identificateurs d’élément ne correspondent pas, vous savez que les données ont été supprimées ou insérées dans les parties de la liste que vous avez déjà « paginées ».</span><span class="sxs-lookup"><span data-stu-id="cd143-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="cd143-206">Même lorsque vous savez que les données ont changé, vous devez quand même décider comment réagir.</span><span class="sxs-lookup"><span data-stu-id="cd143-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="cd143-207">Il n’y a pas non plus de réponse universelle à cette question.</span><span class="sxs-lookup"><span data-stu-id="cd143-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="cd143-208">Vos actions dépendront de la nature de votre application et de l’importance de capturer tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="cd143-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="cd143-209">Vous pouvez l’ignorer complètement, redémarrer le processus depuis le début ou revenir en arrière et essayer de détecter où le changement s’est produit.</span><span class="sxs-lookup"><span data-stu-id="cd143-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="cd143-210">Exemple : effectuer une recherche paginée à l’aide de l’API gérée EWS</span><span class="sxs-lookup"><span data-stu-id="cd143-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="cd143-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cd143-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="cd143-212">La pagination est prise en charge par les méthodes de l’API gérée EWS suivantes :</span><span class="sxs-lookup"><span data-stu-id="cd143-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="cd143-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="cd143-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="cd143-217">Si vous utilisez l’API gérée EWS, votre application configure la pagination avec la classe [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou la classe [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit les informations du serveur concernant la pagination de la classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou de la classe [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd143-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="cd143-218">L’exemple suivant récupère tous les éléments d’un dossier à l’aide d’une recherche paginée qui renvoie cinq éléments dans chaque réponse.</span><span class="sxs-lookup"><span data-stu-id="cd143-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="cd143-219">Il récupère également un élément supplémentaire pour servir d’ancre afin de détecter les modifications des résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="cd143-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="cd143-220">Cet exemple suppose que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les propriétés [Identifiants](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd143-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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
            if (moreItems && anchorId != null)
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
            int displayCount = 0;
            if ((results.MoreAvailable == false && results.Items.Count > pageSize) || (results.Items.Count < pageSize))
            {
                displayCount = results.Items.Count;
            }
            else
            {
                displayCount = pageSize;
            }
            
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

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="cd143-221">Exemple : effectuer une recherche paginée à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="cd143-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="cd143-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cd143-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="cd143-223">La pagination est prise en charge par les opérations EWS suivantes :</span><span class="sxs-lookup"><span data-stu-id="cd143-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="cd143-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="cd143-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="cd143-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="cd143-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="cd143-226">Si vous utilisez EWS, votre application configure la pagination avec l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit les informations du serveur concernant la pagination de l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou de l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cd143-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="cd143-227">Dans cet exemple de demande, une demande **FindItem** est envoyée pour un maximum de six éléments, en commençant avec un décalage de zéro à partir du début de la liste des éléments dans la boîte de réception de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cd143-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
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

<span data-ttu-id="cd143-228">Le serveur renvoie la réponse suivante, qui contient six éléments.</span><span class="sxs-lookup"><span data-stu-id="cd143-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="cd143-229">La réponse indique également qu’il y a un total de huit éléments dans les résultats sur le serveur et que le dernier élément de la liste de résultats n’est pas présent dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="cd143-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

<span data-ttu-id="cd143-230">Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut **Offset** passe à cinq, ce qui indique que le serveur doit renvoyer au plus six éléments à partir du décalage de cinq depuis le début.</span><span class="sxs-lookup"><span data-stu-id="cd143-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
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

<span data-ttu-id="cd143-231">Le serveur envoie la réponse suivante, qui contient trois éléments.</span><span class="sxs-lookup"><span data-stu-id="cd143-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="cd143-232">La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours de huit et que le dernier élément de la liste de résultats est inclus dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="cd143-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

## <a name="see-also"></a><span data-ttu-id="cd143-233">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cd143-233">See also</span></span>


- [<span data-ttu-id="cd143-234">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cd143-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="cd143-235">Méthode ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-236">Méthode ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="cd143-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-237">Méthode Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-238">Méthode Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="cd143-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cd143-239">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="cd143-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="cd143-240">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="cd143-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="cd143-241">Limitation EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cd143-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

