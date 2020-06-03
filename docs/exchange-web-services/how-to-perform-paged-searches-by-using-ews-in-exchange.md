---
title: Effectuer des recherches paginées à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Découvrez comment effectuer des recherches paginées dans votre API managée EWS ou votre application EWS qui cible Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b608584918c936f62883b8b444d59c05c5952ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456833"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="1382d-103">Effectuer des recherches paginées à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1382d-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="1382d-104">Découvrez comment effectuer des recherches paginées dans votre API managée EWS ou votre application EWS qui cible Exchange.</span><span class="sxs-lookup"><span data-stu-id="1382d-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="1382d-105">La pagination est une fonctionnalité d’EWS qui vous permet de contrôler la taille des résultats d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="1382d-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="1382d-106">Au lieu de récupérer l’intégralité du jeu de résultats dans une réponse EWS, vous pouvez récupérer des jeux plus petits dans plusieurs réponses EWS.</span><span class="sxs-lookup"><span data-stu-id="1382d-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="1382d-107">Par exemple, imaginons qu’un utilisateur dispose de 10 000 messages électroniques dans sa boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="1382d-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="1382d-108">De manière hypothétique, vous pouviez extraire tous les courriers électroniques de 10 000 en une seule très grande réponse, mais vous pouvez le diviser en morceaux plus faciles à gérer pour des raisons de performances ou de bande passante.</span><span class="sxs-lookup"><span data-stu-id="1382d-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="1382d-109">La pagination vous offre les outils qui vous permettent d’effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="1382d-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1382d-110">Bien que vous puissiez généralement extraire 10 000 éléments dans une demande, en réalité, cela est improbable en raison de la limitation EWS.</span><span class="sxs-lookup"><span data-stu-id="1382d-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="1382d-111">Pour en savoir plus, reportez-vous à la rubrique [limitation EWS dans Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="1382d-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="1382d-112">**Tableau 1. Paramètres de pagination dans l’API managée EWS et EWS**</span><span class="sxs-lookup"><span data-stu-id="1382d-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="1382d-113">**Pour configurer ou récupérer le...**</span><span class="sxs-lookup"><span data-stu-id="1382d-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="1382d-114">**Dans l’API managée EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="1382d-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="1382d-115">**Dans EWS, utilisez...**</span><span class="sxs-lookup"><span data-stu-id="1382d-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1382d-116">Nombre maximal d’éléments ou de dossiers dans une réponse</span><span class="sxs-lookup"><span data-stu-id="1382d-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="1382d-117">Le paramètre **pageSize** vers le [constructeur objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou le [constructeur folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="1382d-118">Ou</span><span class="sxs-lookup"><span data-stu-id="1382d-118">Or</span></span>  <br/> <span data-ttu-id="1382d-119">Propriété [PagedView. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-120">Attribut **MaxEntriesReturned** de l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou de l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="1382d-121">Point de départ dans la liste d’éléments ou de dossiers</span><span class="sxs-lookup"><span data-stu-id="1382d-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="1382d-122">Le paramètre **offsetBasePoint** pour le constructeur **objetitemview** ou le constructeur **folderview**</span><span class="sxs-lookup"><span data-stu-id="1382d-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="1382d-123">Ou</span><span class="sxs-lookup"><span data-stu-id="1382d-123">Or</span></span>  <br/> <span data-ttu-id="1382d-124">Propriété [PagedView. OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-125">Attribut **BasePoint** de l’élément **IndexedPageItemView** ou de l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="1382d-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="1382d-126">Décalage depuis le point de départ</span><span class="sxs-lookup"><span data-stu-id="1382d-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="1382d-127">Le paramètre **offset** pour le constructeur **objetitemview** ou le constructeur **folderview**</span><span class="sxs-lookup"><span data-stu-id="1382d-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="1382d-128">Ou</span><span class="sxs-lookup"><span data-stu-id="1382d-128">Or</span></span>  <br/> <span data-ttu-id="1382d-129">Propriété [PagedView. Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-130">L’attribut **offset** sur l’élément **IndexedPageItemView** ou l’élément **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="1382d-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="1382d-131">Nombre total de résultats sur le serveur</span><span class="sxs-lookup"><span data-stu-id="1382d-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="1382d-132">La propriété [FindItemsResults. TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-133">L’attribut **TotalItemsInView** sur l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="1382d-134">Décalage du premier élément ou du dossier non inclus dans la réponse actuelle</span><span class="sxs-lookup"><span data-stu-id="1382d-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="1382d-135">La propriété [FindItemsResults. NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-136">Attribut **IndexedPagingOffset** de l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="1382d-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="1382d-137">Indicateur indiquant que la réponse inclut le dernier élément ou dossier de la liste</span><span class="sxs-lookup"><span data-stu-id="1382d-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="1382d-138">La propriété [FindItemsResults. MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou la propriété [FindFoldersResults. MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1382d-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="1382d-139">Attribut **IncludesLastItemInRange** de l’élément **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="1382d-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="1382d-140">Fonctionnement de la pagination</span><span class="sxs-lookup"><span data-stu-id="1382d-140">How paging works</span></span>
<span data-ttu-id="1382d-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="1382d-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="1382d-142">Pour comprendre le fonctionnement de la pagination, il est utile de visualiser les messages d’un dossier sous forme de panneaux alignés côte à côte dans un champ extérieur à votre maison.</span><span class="sxs-lookup"><span data-stu-id="1382d-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="1382d-143">Vous pouvez voir certains de ces panneaux dans une fenêtre magique.</span><span class="sxs-lookup"><span data-stu-id="1382d-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="1382d-144">Vous avez la possibilité de modifier la taille de la fenêtre (pour afficher plus ou moins de panneaux d’affichage en même temps) et de déplacer la fenêtre (afin de contrôler les panneaux des panneaux que vous pouvez voir).</span><span class="sxs-lookup"><span data-stu-id="1382d-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="1382d-145">Cette manipulation de la fenêtre est la pagination.</span><span class="sxs-lookup"><span data-stu-id="1382d-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="1382d-146">Lorsque vous envoyez votre demande au serveur Exchange, vous spécifiez la taille de votre fenêtre en termes de nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="1382d-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="1382d-147">Vous définissez la position de la fenêtre en spécifiant un point de départ (au début de la ligne ou à la fin de la ligne) et un décalage par rapport à ce point de départ, exprimé par un certain nombre d’éléments.</span><span class="sxs-lookup"><span data-stu-id="1382d-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="1382d-148">Le début de la fenêtre est le nombre d’éléments spécifié par le décalage à partir du point de départ.</span><span class="sxs-lookup"><span data-stu-id="1382d-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="1382d-149">Lorsque la pagination obtient un peu plus attrayant se trouve dans la réponse du serveur et comment votre application peut utiliser cette réponse pour adapter sa requête suivante.</span><span class="sxs-lookup"><span data-stu-id="1382d-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="1382d-150">Le serveur vous fournit trois informations que vous pouvez utiliser pour déterminer la procédure à suivre pour configurer votre « fenêtre » pour votre prochaine requête :</span><span class="sxs-lookup"><span data-stu-id="1382d-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="1382d-151">Indique si les résultats dans la réponse incluent le dernier élément dans l’ensemble de résultats global sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="1382d-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="1382d-152">Nombre total d’éléments dans le jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="1382d-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="1382d-153">La valeur de décalage suivante, si vous souhaitez faire avancer votre fenêtre à l’élément suivant dans le jeu de résultats qui n’est pas inclus dans la réponse actuelle.</span><span class="sxs-lookup"><span data-stu-id="1382d-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="1382d-154">Examinons un exemple simple.</span><span class="sxs-lookup"><span data-stu-id="1382d-154">Let's look at a simple example.</span></span> <span data-ttu-id="1382d-155">Imaginez une boîte de réception comportant 15 messages.</span><span class="sxs-lookup"><span data-stu-id="1382d-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="1382d-156">Votre application envoie une demande initiale pour extraire un maximum de 10 éléments, en commençant au début de la liste des messages (de sorte que le décalage est égal à zéro).</span><span class="sxs-lookup"><span data-stu-id="1382d-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="1382d-157">Le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a au total 15 éléments, et que le prochain décalage doit être de 10.</span><span class="sxs-lookup"><span data-stu-id="1382d-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="1382d-158">**Figure 1. Demande de 10 éléments au décalage 0 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="1382d-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 0 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="1382d-160">Votre application renvoie ensuite la même demande au serveur, avec la seule modification dont le décalage est désormais égal à 10.</span><span class="sxs-lookup"><span data-stu-id="1382d-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="1382d-161">Le serveur renvoie les cinq derniers éléments, et indique que la réponse inclut le dernier élément, qu’il y a au total 15 éléments, et que le prochain décalage doit être 15 (bien entendu, vous avez atteint la fin, de sorte qu’il n’y aura pas de décalage suivant.)</span><span class="sxs-lookup"><span data-stu-id="1382d-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="1382d-162">**Figure 2. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments**</span><span class="sxs-lookup"><span data-stu-id="1382d-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 15 éléments.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="1382d-164">Considérations relatives à la conception pour la pagination</span><span class="sxs-lookup"><span data-stu-id="1382d-164">Design considerations for paging</span></span>
<span data-ttu-id="1382d-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="1382d-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="1382d-166">Pour tirer le meilleur parti de la pagination dans votre application, vous devez tenir compte de la nécessité.</span><span class="sxs-lookup"><span data-stu-id="1382d-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="1382d-167">Par exemple, quelle est la taille de votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="1382d-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="1382d-168">Que faire si les résultats sur le serveur changent pendant que vous déplacez votre « fenêtre » ?</span><span class="sxs-lookup"><span data-stu-id="1382d-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="1382d-169">Déterminer la taille de votre fenêtre</span><span class="sxs-lookup"><span data-stu-id="1382d-169">Determine the size of your window</span></span>

<span data-ttu-id="1382d-170">Il n’existe pas de nombre maximal d’entrées « à taille unique » que toutes les applications doivent utiliser.</span><span class="sxs-lookup"><span data-stu-id="1382d-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="1382d-171">La détermination du nombre correct pour votre application dépend de plusieurs facteurs.</span><span class="sxs-lookup"><span data-stu-id="1382d-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="1382d-172">Toutefois, il est utile de garder à l’esprit les instructions suivantes :</span><span class="sxs-lookup"><span data-stu-id="1382d-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="1382d-173">Par défaut, Exchange limite le nombre maximal d’éléments qui peuvent être renvoyés dans une demande unique à 1000.</span><span class="sxs-lookup"><span data-stu-id="1382d-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="1382d-174">Le fait de définir le nombre maximal d’entrées sur un nombre plus élevé entraîne l’envoi de moins de demandes pour obtenir tous les éléments, au coût de l’attente de réponses plus longues.</span><span class="sxs-lookup"><span data-stu-id="1382d-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="1382d-175">Le fait de définir le nombre maximal d’entrées sur un nombre inférieur entraîne des temps de réponse plus rapides, au prix de l’envoi de demandes supplémentaires pour obtenir tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="1382d-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="1382d-176">Gestion des modifications apportées au jeu de résultats</span><span class="sxs-lookup"><span data-stu-id="1382d-176">Handling changes to the result set</span></span>

<span data-ttu-id="1382d-177">Dans l’exemple simple plus haut dans cet article, le nombre d’éléments dans la boîte de réception de l’utilisateur restait constant.</span><span class="sxs-lookup"><span data-stu-id="1382d-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="1382d-178">Toutefois, en réalité, le nombre d’éléments dans une boîte de réception peut changer fréquemment.</span><span class="sxs-lookup"><span data-stu-id="1382d-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="1382d-179">Les nouveaux messages peuvent arriver et les éléments peuvent être supprimés ou déplacés à tout moment.</span><span class="sxs-lookup"><span data-stu-id="1382d-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="1382d-180">En quoi cela affecte-t-il la pagination ?</span><span class="sxs-lookup"><span data-stu-id="1382d-180">But how does this impact paging?</span></span> <span data-ttu-id="1382d-181">Nous allons modifier l’exemple de scénario précédent pour le savoir.</span><span class="sxs-lookup"><span data-stu-id="1382d-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="1382d-182">Nous allons redémarrer avec les 15 éléments dans la boîte de réception de l’utilisateur, puis envoyer la même demande initiale.</span><span class="sxs-lookup"><span data-stu-id="1382d-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="1382d-183">Comme précédemment, le serveur répond avec les 10 premiers messages et indique que la réponse n’inclut pas le dernier élément, qu’il y a un total de 15 éléments, et que le décalage suivant doit être de 10, comme illustré dans la figure 1.</span><span class="sxs-lookup"><span data-stu-id="1382d-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="1382d-184">Maintenant, pendant que votre application traite ces 10 éléments, un nouveau message arrive dans la boîte de réception et est ajouté au jeu de résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="1382d-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="1382d-185">Votre application renvoie la même demande au serveur (uniquement avec le décalage défini sur 10).</span><span class="sxs-lookup"><span data-stu-id="1382d-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="1382d-186">Cette fois, le serveur renvoie six éléments et indique qu’il y a au total 16 éléments dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="1382d-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="1382d-187">À ce stade, vous vous demandez s’il s’agit d’un problème même.</span><span class="sxs-lookup"><span data-stu-id="1382d-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="1382d-188">Après tout, vous avez 16 éléments sur les deux réponses, alors pourquoi tout ça ?</span><span class="sxs-lookup"><span data-stu-id="1382d-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="1382d-189">La réponse dépend de l’emplacement du nouvel élément dans la liste.</span><span class="sxs-lookup"><span data-stu-id="1382d-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="1382d-190">Si la liste est triée de façon à ce que les éléments les plus anciens (par date/heure de réception) soient les premiers, il n’y a aucune cause de préoccupation dans ce scénario.</span><span class="sxs-lookup"><span data-stu-id="1382d-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="1382d-191">Le nouvel élément sera placé à la fin de la liste et sera inclus dans la deuxième réponse.</span><span class="sxs-lookup"><span data-stu-id="1382d-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="1382d-192">**Figure 3. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le 16ème élément de la liste en cours de nouvelle**</span><span class="sxs-lookup"><span data-stu-id="1382d-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments quand le 16e élément a été ajouté à la fin de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="1382d-194">Si la liste est triée de sorte que les éléments les plus récents soient les premiers, il s’agit d’un autre article.</span><span class="sxs-lookup"><span data-stu-id="1382d-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="1382d-195">Dans ce cas, le premier élément de la deuxième requête est le dernier élément de la requête précédente plus les cinq éléments restants du 15 initial.</span><span class="sxs-lookup"><span data-stu-id="1382d-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="1382d-196">Pour le placer en tant que fenêtre magique imaginaire, vous avez déplacé la position de votre fenêtre de 10, mais les panneaux ont eux-mêmes également été décalés de 1.</span><span class="sxs-lookup"><span data-stu-id="1382d-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="1382d-197">**Figure 4. Demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments, avec le premier élément de la liste en cours de nouvelle**</span><span class="sxs-lookup"><span data-stu-id="1382d-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![Diagramme présentant les résultats d’une demande de 10 éléments au décalage de 10 à partir du début d’une liste de 16 éléments lorsque le 16e élément a été ajouté au début de la liste.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="1382d-199">Pour détecter une modification apportée aux résultats sur le serveur, vous pouvez utiliser le concept d’un élément d’ancrage.</span><span class="sxs-lookup"><span data-stu-id="1382d-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="1382d-200">Un élément d’ancrage est un élément supplémentaire de votre réponse qui n’est pas traité avec le reste des résultats, mais qui est utilisé pour comparer avec les résultats suivants pour voir si les éléments eux-mêmes ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="1382d-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="1382d-201">Si votre application utilise une taille de 10, vous pouvez définir le nombre maximal d’éléments à 11, si votre application utilise une taille de « fenêtre ».</span><span class="sxs-lookup"><span data-stu-id="1382d-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="1382d-202">Votre application traite les 10 premiers éléments de la réponse comme d’habitude.</span><span class="sxs-lookup"><span data-stu-id="1382d-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="1382d-203">Pour le dernier élément, enregistrez l’identificateur de l’élément en tant qu’ancre, puis émettez la requête suivante avec un décalage de 10.</span><span class="sxs-lookup"><span data-stu-id="1382d-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="1382d-204">Si les données n’ont pas été modifiées, le premier élément de la deuxième réponse doit avoir un identificateur d’élément correspondant à l’ancre.</span><span class="sxs-lookup"><span data-stu-id="1382d-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="1382d-205">Si les identificateurs d’élément ne correspondent pas, cela signifie que les données ont été supprimées ou insérées dans les parties de la liste que vous avez déjà « paginée ».</span><span class="sxs-lookup"><span data-stu-id="1382d-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="1382d-206">Même si vous êtes conscient que les données ont été modifiées, vous devez toujours décider comment réagir.</span><span class="sxs-lookup"><span data-stu-id="1382d-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="1382d-207">Il n’y a pas de réponse à une seule taille pour cette question.</span><span class="sxs-lookup"><span data-stu-id="1382d-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="1382d-208">Vos actions dépendent de la nature de votre application et de l’importance de la capture de tous les éléments.</span><span class="sxs-lookup"><span data-stu-id="1382d-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="1382d-209">Vous pouvez l’ignorer, redémarrez le processus depuis le début ou l’arrière et essayez de détecter où la modification s’est produite.</span><span class="sxs-lookup"><span data-stu-id="1382d-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="1382d-210">Exemple : effectuer une recherche paginée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="1382d-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="1382d-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="1382d-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="1382d-212">La pagination est prise en charge par les méthodes d’API managée EWS suivantes :</span><span class="sxs-lookup"><span data-stu-id="1382d-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="1382d-213">ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-214">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="1382d-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-215">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-216">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="1382d-217">Si vous utilisez l’API managée EWS, votre application configure la pagination à l’aide de la classe [objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) et reçoit des informations du serveur concernant la pagination à partir de la classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1382d-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="1382d-218">L’exemple suivant récupère tous les éléments d’un dossier à l’aide d’une recherche paginée qui renvoie cinq éléments dans chaque réponse.</span><span class="sxs-lookup"><span data-stu-id="1382d-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="1382d-219">Il extrait également un élément supplémentaire qui servira d’ancre pour détecter les modifications apportées aux résultats sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="1382d-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="1382d-220">Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1382d-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="1382d-221">Exemple : effectuer une recherche paginée à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="1382d-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="1382d-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="1382d-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="1382d-223">La pagination est prise en charge par les opérations EWS suivantes :</span><span class="sxs-lookup"><span data-stu-id="1382d-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="1382d-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="1382d-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="1382d-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="1382d-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="1382d-226">Si vous utilisez EWS, votre application configure la pagination avec l’élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou l’élément [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) et reçoit des informations du serveur concernant la pagination à partir de l’élément [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou de l’élément [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1382d-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="1382d-227">Dans cet exemple de requête, une requête **FindItem** est envoyée pour un maximum de six éléments, en commençant à un offset de zéro à partir du début de la liste des éléments dans la boîte de réception de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1382d-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
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

<span data-ttu-id="1382d-228">Le serveur renvoie la réponse suivante, qui contient six éléments.</span><span class="sxs-lookup"><span data-stu-id="1382d-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="1382d-229">La réponse indique également qu’il y a au total huit éléments dans les résultats sur le serveur, et que le dernier élément de la liste des résultats n’est pas présent dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="1382d-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
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

<span data-ttu-id="1382d-230">Dans cet exemple, la même demande est envoyée, mais cette fois, l’attribut **offset** est remplacé par cinq, ce qui indique que le serveur doit renvoyer au plus six éléments en commençant au décalage cinq depuis le début.</span><span class="sxs-lookup"><span data-stu-id="1382d-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
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

<span data-ttu-id="1382d-231">Le serveur envoie la réponse suivante, qui contient trois éléments.</span><span class="sxs-lookup"><span data-stu-id="1382d-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="1382d-232">La réponse indique également que le nombre total d’éléments dans les résultats sur le serveur est toujours huit et que le dernier élément de la liste de résultats est inclus dans cette réponse.</span><span class="sxs-lookup"><span data-stu-id="1382d-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="1382d-233">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1382d-233">See also</span></span>


- [<span data-ttu-id="1382d-234">Recherche et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1382d-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="1382d-235">Méthode ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-236">Méthode ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="1382d-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-237">Méthode Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-238">Méthode Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="1382d-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1382d-239">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="1382d-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="1382d-240">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="1382d-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="1382d-241">Limitation EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1382d-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

