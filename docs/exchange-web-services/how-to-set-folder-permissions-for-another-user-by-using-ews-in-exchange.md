---
title: Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: e25f1a49a430e8c95829d404fa53451b76cab167
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455869"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="ba2a5-103">Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="ba2a5-104">Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="ba2a5-105">Les autorisations au niveau du dossier permettent aux utilisateurs d’accéder à un ou plusieurs dossiers dans la boîte aux lettres d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="ba2a5-106">Les autorisations de dossier sont semblables à l’accès délégué, mais elles diffèrent de la façon suivante :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="ba2a5-107">Les autorisations de dossier ne permettent pas à un utilisateur de « envoyer de la part de » ou « envoyer en tant que » un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="ba2a5-108">Ils autorisent uniquement l’accès aux dossiers.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-108">They only enable access to folders.</span></span> <span data-ttu-id="ba2a5-109">Les utilisateurs peuvent créer des éléments dans ces dossiers, mais ils ne peuvent pas les envoyer.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="ba2a5-110">Vous pouvez définir des autorisations de dossier sur n’importe quel dossier de la boîte aux lettres, mais vous ne pouvez ajouter un délégué qu’aux dossiers calendrier, contacts, boîte de réception, Journal, notes et tâches.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="ba2a5-111">Vous pouvez définir un certain nombre d' [autorisations sur un dossier spécifique](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="ba2a5-112">Lorsque vous ajoutez un délégué, vous pouvez affecter l’un des [cinq niveaux d’autorisation](delegate-access-and-ews-in-exchange.md#bk_delegateperms)seulement.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="ba2a5-113">Vous pouvez définir des autorisations de dossier pour les utilisateurs anonymes et par défaut.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="ba2a5-114">Vous pouvez uniquement accorder l’accès délégué à un compte à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="ba2a5-115">Si vous êtes familiarisé avec les entrées de contrôle d’accès (ACE) et les listes de contrôle d’accès discrétionnaire (DACL), vous savez qu’un utilisateur ne peut avoir qu’un seul ensemble d’autorisations pour chaque dossier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="ba2a5-116">Si vous essayez d’ajouter un jeu d’autorisations pour un utilisateur et qu’ils disposent déjà d’un ensemble d’autorisations, vous obtiendrez une erreur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="ba2a5-117">Lorsque vous ajoutez, supprimez ou mettez à jour des autorisations sur un dossier, vous obtenez la liste DACL actuelle, ajoutez ou supprimez des ACE, puis envoyez la liste DACL mise à jour.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="ba2a5-118">Vous ne pouvez pas ajouter plusieurs ACE pour le même utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="ba2a5-119">Lorsque vous mettez à jour les autorisations à l’aide de l’API managée EWS, vous devez supprimer l’ACE actuelle de l’utilisateur, puis ajouter sa nouvelle ACE à la collection.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="ba2a5-120">Si vous utilisez EWS, il vous suffit de remplacer le jeu d’ACE précédent par le nouveau.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="ba2a5-121">Si vous apportez plusieurs modifications d’autorisations à un seul dossier, vous pouvez effectuer des ajouts, des suppressions ou des mises à jour par lot, mais notez simplement que vous ne pouvez pas effectuer de mises à jour par lots sur plusieurs dossiers.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="ba2a5-122">Un appel est nécessaire pour obtenir les autorisations sur un seul dossier, et un deuxième appel est nécessaire pour mettre à jour les autorisations sur ce dossier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="ba2a5-123">Lorsque vous ajoutez, supprimez ou mettez à jour des autorisations utilisateur, vous utilisez les deux mêmes appels ou opérations de méthode pour chaque tâche.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="ba2a5-124">**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour la définition des autorisations de dossier**</span><span class="sxs-lookup"><span data-stu-id="ba2a5-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="ba2a5-125">Si vous souhaitez...</span><span class="sxs-lookup"><span data-stu-id="ba2a5-125">If you want to…</span></span>|<span data-ttu-id="ba2a5-126">Utilisez cette méthode d’API managée EWS...</span><span class="sxs-lookup"><span data-stu-id="ba2a5-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="ba2a5-127">Utilisez cette opération EWS...</span><span class="sxs-lookup"><span data-stu-id="ba2a5-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ba2a5-128">Activer, supprimer ou mettre à jour les autorisations de dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="ba2a5-129">[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi de [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-129">[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="ba2a5-130">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) suivi par [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-130">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="ba2a5-131">Création d’un dossier et définition des autorisations de dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="ba2a5-132">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="ba2a5-132">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ba2a5-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="ba2a5-133">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="ba2a5-134">Autorisations d’accès aux dossiers</span><span class="sxs-lookup"><span data-stu-id="ba2a5-134">Folder permissions</span></span>
<span data-ttu-id="ba2a5-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-135"><a name="bk_folderperms"> </a></span></span>

<span data-ttu-id="ba2a5-136">Vous disposez de plusieurs options pour définir des autorisations de dossier sur un dossier spécifique.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="ba2a5-137">Vous pouvez définir un niveau d’autorisation sur un dossier pour chaque utilisateur, ce qui ajoute un ensemble d’autorisations individuelles prédéfinies à la liste DACL, ou vous pouvez définir des autorisations individuelles sur un dossier, mais vous ne pouvez pas mélanger et faire correspondre.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="ba2a5-138">Les autorisations individuelles suivantes sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="ba2a5-139">Pouvez créer</span><span class="sxs-lookup"><span data-stu-id="ba2a5-139">Can create</span></span>
- <span data-ttu-id="ba2a5-140">Possibilité de créer des sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="ba2a5-140">Can create subfolders</span></span>    
- <span data-ttu-id="ba2a5-141">Est le propriétaire du dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-141">Is folder owner</span></span>    
- <span data-ttu-id="ba2a5-142">Le dossier est-il visible</span><span class="sxs-lookup"><span data-stu-id="ba2a5-142">Is folder visible</span></span>    
- <span data-ttu-id="ba2a5-143">Est le contact du dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-143">Is folder contact</span></span>    
- <span data-ttu-id="ba2a5-144">Modifier des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-144">Edit items</span></span>    
- <span data-ttu-id="ba2a5-145">Supprimer des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-145">Delete items</span></span>    
- <span data-ttu-id="ba2a5-146">Lire des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-146">Read items</span></span>
    
<span data-ttu-id="ba2a5-147">En outre, les niveaux d’autorisation suivants sont disponibles, qui définissent un sous-ensemble des autorisations et des valeurs individuelles, comme indiqué dans le tableau 2 :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="ba2a5-148">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-148">None</span></span>    
- <span data-ttu-id="ba2a5-149">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="ba2a5-149">Owner</span></span>    
- <span data-ttu-id="ba2a5-150">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-150">PublishingEditor</span></span>    
- <span data-ttu-id="ba2a5-151">Éditeur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-151">Editor</span></span>    
- <span data-ttu-id="ba2a5-152">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-152">PublishingAuthor</span></span>    
- <span data-ttu-id="ba2a5-153">Auteur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-153">Author</span></span>    
- <span data-ttu-id="ba2a5-154">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="ba2a5-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="ba2a5-155">Relecteur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-155">Reviewer</span></span>    
- <span data-ttu-id="ba2a5-156">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-156">Contributor</span></span>   
- <span data-ttu-id="ba2a5-157">Custom : cette valeur ne peut pas être définie par l’application.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="ba2a5-158">Le serveur définit cette valeur si l’application inclut une collection personnalisée d’autorisations individuelles.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="ba2a5-159">FreeBusyTimeOnly-cette valeur ne peut être définie que sur les dossiers de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="ba2a5-160">FreeBusyTimeAndSubjectAndLocation-cette valeur ne peut être définie que sur les dossiers de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="ba2a5-161">Le tableau suivant indique les autorisations individuelles qui sont appliquées par défaut en fonction du niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="ba2a5-162">**Tableau 2. Autorisations individuelles par niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="ba2a5-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="ba2a5-163">Niveau d’autorisation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-163">Permission level</span></span>|<span data-ttu-id="ba2a5-164">Peut créer des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-164">Can create items</span></span>|<span data-ttu-id="ba2a5-165">Possibilité de créer des sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="ba2a5-165">Can create sub folders</span></span>|<span data-ttu-id="ba2a5-166">Est le propriétaire du dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-166">Is folder owner</span></span>|<span data-ttu-id="ba2a5-167">Le dossier est-il visible</span><span class="sxs-lookup"><span data-stu-id="ba2a5-167">Is folder visible</span></span>|<span data-ttu-id="ba2a5-168">Est le contact du dossier</span><span class="sxs-lookup"><span data-stu-id="ba2a5-168">Is folder contact</span></span>|<span data-ttu-id="ba2a5-169">Modifier des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-169">Edit items</span></span>|<span data-ttu-id="ba2a5-170">Supprimer des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-170">Delete items</span></span>|<span data-ttu-id="ba2a5-171">Peut lire des éléments</span><span class="sxs-lookup"><span data-stu-id="ba2a5-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="ba2a5-172">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-172">None</span></span>  <br/> |<span data-ttu-id="ba2a5-173">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-173">False</span></span>  <br/> |<span data-ttu-id="ba2a5-174">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-174">False</span></span>  <br/> |<span data-ttu-id="ba2a5-175">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-175">False</span></span>  <br/> |<span data-ttu-id="ba2a5-176">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-176">False</span></span>  <br/> |<span data-ttu-id="ba2a5-177">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-177">False</span></span>  <br/> |<span data-ttu-id="ba2a5-178">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-178">None</span></span>  <br/> |<span data-ttu-id="ba2a5-179">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-179">None</span></span>  <br/> |<span data-ttu-id="ba2a5-180">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-180">None</span></span>  <br/> |
|<span data-ttu-id="ba2a5-181">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="ba2a5-181">Owner</span></span>  <br/> |<span data-ttu-id="ba2a5-182">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-182">True</span></span>  <br/> |<span data-ttu-id="ba2a5-183">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-183">True</span></span>  <br/> |<span data-ttu-id="ba2a5-184">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-184">True</span></span>  <br/> |<span data-ttu-id="ba2a5-185">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-185">True</span></span>  <br/> |<span data-ttu-id="ba2a5-186">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-186">True</span></span>  <br/> |<span data-ttu-id="ba2a5-187">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-187">All</span></span>  <br/> |<span data-ttu-id="ba2a5-188">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-188">All</span></span>  <br/> |<span data-ttu-id="ba2a5-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-190">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="ba2a5-191">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-191">True</span></span>  <br/> |<span data-ttu-id="ba2a5-192">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-192">True</span></span>  <br/> |<span data-ttu-id="ba2a5-193">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-193">False</span></span>  <br/> |<span data-ttu-id="ba2a5-194">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-194">True</span></span>  <br/> |<span data-ttu-id="ba2a5-195">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-195">False</span></span>  <br/> |<span data-ttu-id="ba2a5-196">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-196">All</span></span>  <br/> |<span data-ttu-id="ba2a5-197">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-197">All</span></span>  <br/> |<span data-ttu-id="ba2a5-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-199">Éditeur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-199">Editor</span></span>  <br/> |<span data-ttu-id="ba2a5-200">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-200">True</span></span>  <br/> |<span data-ttu-id="ba2a5-201">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-201">False</span></span>  <br/> |<span data-ttu-id="ba2a5-202">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-202">False</span></span>  <br/> |<span data-ttu-id="ba2a5-203">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-203">True</span></span>  <br/> |<span data-ttu-id="ba2a5-204">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-204">False</span></span>  <br/> |<span data-ttu-id="ba2a5-205">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-205">All</span></span>  <br/> |<span data-ttu-id="ba2a5-206">Tous</span><span class="sxs-lookup"><span data-stu-id="ba2a5-206">All</span></span>  <br/> |<span data-ttu-id="ba2a5-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-208">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="ba2a5-209">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-209">True</span></span>  <br/> |<span data-ttu-id="ba2a5-210">True</span><span class="sxs-lookup"><span data-stu-id="ba2a5-210">True</span></span>  <br/> |<span data-ttu-id="ba2a5-211">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-211">False</span></span>  <br/> |<span data-ttu-id="ba2a5-212">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-212">True</span></span>  <br/> |<span data-ttu-id="ba2a5-213">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-213">False</span></span>  <br/> |<span data-ttu-id="ba2a5-214">Appartien</span><span class="sxs-lookup"><span data-stu-id="ba2a5-214">Owned</span></span>  <br/> |<span data-ttu-id="ba2a5-215">Appartien</span><span class="sxs-lookup"><span data-stu-id="ba2a5-215">Owned</span></span>  <br/> |<span data-ttu-id="ba2a5-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-217">Auteur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-217">Author</span></span>  <br/> |<span data-ttu-id="ba2a5-218">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-218">True</span></span>  <br/> |<span data-ttu-id="ba2a5-219">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-219">False</span></span>  <br/> |<span data-ttu-id="ba2a5-220">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-220">False</span></span>  <br/> |<span data-ttu-id="ba2a5-221">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-221">True</span></span>  <br/> |<span data-ttu-id="ba2a5-222">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-222">False</span></span>  <br/> |<span data-ttu-id="ba2a5-223">Appartien</span><span class="sxs-lookup"><span data-stu-id="ba2a5-223">Owned</span></span>  <br/> |<span data-ttu-id="ba2a5-224">Appartien</span><span class="sxs-lookup"><span data-stu-id="ba2a5-224">Owned</span></span>  <br/> |<span data-ttu-id="ba2a5-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-226">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="ba2a5-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="ba2a5-227">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-227">True</span></span>  <br/> |<span data-ttu-id="ba2a5-228">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-228">False</span></span>  <br/> |<span data-ttu-id="ba2a5-229">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-229">False</span></span>  <br/> |<span data-ttu-id="ba2a5-230">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-230">True</span></span>  <br/> |<span data-ttu-id="ba2a5-231">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-231">False</span></span>  <br/> |<span data-ttu-id="ba2a5-232">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-232">None</span></span>  <br/> |<span data-ttu-id="ba2a5-233">Appartien</span><span class="sxs-lookup"><span data-stu-id="ba2a5-233">Owned</span></span>  <br/> |<span data-ttu-id="ba2a5-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-235">Relecteur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-235">Reviewer</span></span>  <br/> |<span data-ttu-id="ba2a5-236">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-236">False</span></span>  <br/> |<span data-ttu-id="ba2a5-237">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-237">False</span></span>  <br/> |<span data-ttu-id="ba2a5-238">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-238">False</span></span>  <br/> |<span data-ttu-id="ba2a5-239">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-239">True</span></span>  <br/> |<span data-ttu-id="ba2a5-240">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-240">False</span></span>  <br/> |<span data-ttu-id="ba2a5-241">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-241">None</span></span>  <br/> |<span data-ttu-id="ba2a5-242">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-242">None</span></span>  <br/> |<span data-ttu-id="ba2a5-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ba2a5-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="ba2a5-244">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="ba2a5-244">Contributor</span></span>  <br/> |<span data-ttu-id="ba2a5-245">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-245">True</span></span>  <br/> |<span data-ttu-id="ba2a5-246">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-246">False</span></span>  <br/> |<span data-ttu-id="ba2a5-247">False</span><span class="sxs-lookup"><span data-stu-id="ba2a5-247">False</span></span>  <br/> |<span data-ttu-id="ba2a5-248">Vrai</span><span class="sxs-lookup"><span data-stu-id="ba2a5-248">True</span></span>  <br/> |<span data-ttu-id="ba2a5-249">Faux</span><span class="sxs-lookup"><span data-stu-id="ba2a5-249">False</span></span>  <br/> |<span data-ttu-id="ba2a5-250">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-250">None</span></span>  <br/> |<span data-ttu-id="ba2a5-251">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-251">None</span></span>  <br/> |<span data-ttu-id="ba2a5-252">Aucun</span><span class="sxs-lookup"><span data-stu-id="ba2a5-252">None</span></span>  <br/> |
   
<span data-ttu-id="ba2a5-253">Si vous spécifiez un niveau d’autorisation non personnalisé dans la demande d’autorisations au niveau du dossier, il n’est pas nécessaire de spécifier les paramètres d’autorisation individuels.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="ba2a5-254">Si vous spécifiez une autorisation individuelle lorsque vous définissez un niveau d’autorisation, une erreur **ErrorInvalidPermissionSettings** est renvoyée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="ba2a5-255">Ajout d’autorisations de dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="ba2a5-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-256"><a name="bk_enableewsma"> </a></span></span>

<span data-ttu-id="ba2a5-257">L’exemple de code suivant montre comment utiliser l’API managée EWS pour :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="ba2a5-258">Créez un objet [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) pour le nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-258">Create a new [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="ba2a5-259">Obtenir les autorisations actuelles d’un dossier à l’aide de la méthode [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-259">Get the current permissions for a folder by using the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="ba2a5-260">Ajoutez la nouvelle **FolderPermissions** à la propriété [Folder. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-260">Add the new **FolderPermissions** to the [Folder.Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="ba2a5-261">Appelez la méthode [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les nouvelles autorisations sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-261">Call the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="ba2a5-262">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-262">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

<span data-ttu-id="ba2a5-263">La ligne de code suivante spécifie le niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="ba2a5-264">Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez ce code à la place.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="ba2a5-265">Vous pouvez définir une ou toutes les [Propriétés FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) accessibles en écriture lorsque vous créez un objet **FolderPermission** avec un niveau d’autorisation personnalisé.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-265">You can set any or all of the writable [FolderPermission properties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="ba2a5-266">Notez toutefois que l' [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) n’est jamais définie explicitement sur **Custom** par l’application.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-266">Note, however, that the [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="ba2a5-267">Le **FolderPermissionLevel** est défini sur personnalisé uniquement lorsque vous créez un objet **FolderPermission** et que vous définissez des autorisations individuelles.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="ba2a5-268">Ajout d’autorisations de dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="ba2a5-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-269"><a name="bk_enableews"> </a></span></span>

<span data-ttu-id="ba2a5-270">Les exemples de code EWS suivants montrent comment ajouter des autorisations à un dossier spécifique en extrayant les autorisations actuelles, puis en soumettant une liste de nouvelles autorisations.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="ba2a5-271">La première étape consiste à envoyer une demande [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , dans laquelle la valeur [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) spécifie le dossier dans lequel ajouter des autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut dossier : PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-271">The first step is to send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="ba2a5-272">Cette requête récupère les paramètres d’autorisation pour le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="ba2a5-273">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode **Bind** pour [Ajouter des autorisations de dossier](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="ba2a5-274">Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui inclut la valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le dossier a été récupéré.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-274">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="ba2a5-275">Les valeurs [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) et [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-275">The [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="ba2a5-276">Ensuite, utilisez l’opération **UpdateFolder** pour envoyer le [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)mis à jour, ce qui inclut l' [autorisation](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) pour le nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="ba2a5-277">Notez que l’inclusion de l’élément [SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) pour le dossier respectif dans l’opération [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) remplace tous les paramètres d’autorisation sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-277">Note that including the [SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="ba2a5-278">De même, l’option [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) de l’opération **UpdateFolder** supprimera également tous les paramètres d’autorisation sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-278">Likewise, including the [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="ba2a5-279">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode **Update** pour [Ajouter des autorisations de dossier](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ba2a5-280">La ligne de code suivante spécifie le niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="ba2a5-281">Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez ce code à la place.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-281">If you want to use the custom permission level, use this code instead.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="ba2a5-282">Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le dossier a été mis à jour.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="ba2a5-283">Suppression des autorisations de dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="ba2a5-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-284"><a name="bk_removeewsma"> </a></span></span>

<span data-ttu-id="ba2a5-285">L’exemple de code suivant montre comment utiliser l’API managée EWS pour supprimer toutes les autorisations utilisateur d’un dossier spécifique, à l’exception des autorisations par défaut et anonymes, de la manière suivante :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="ba2a5-286">Obtention des autorisations actuelles pour un dossier à l’aide de la méthode **Bind** .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="ba2a5-287">Itérer au sein de la collection d' **autorisations** et supprimer des autorisations pour des utilisateurs individuels.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="ba2a5-288">Appel de la méthode **Update** pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="ba2a5-289">Cet exemple montre comment supprimer toutes les autorisations utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="ba2a5-290">Si vous souhaitez modifier cet exemple afin de supprimer uniquement les autorisations d’un utilisateur spécifique, modifiez la ligne de code suivante pour identifier le nom complet ou l’adresse SMTP de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="ba2a5-291">Cet exemple part du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié auprès d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-291">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="ba2a5-292">Suppression des autorisations de dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="ba2a5-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-293"><a name="bk_removeews"> </a></span></span>

<span data-ttu-id="ba2a5-294">Les exemples de code EWS suivants montrent comment supprimer toutes les autorisations utilisateur sur un dossier spécifique, à l’exception des autorisations par défaut et anonymes.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="ba2a5-295">Tout d’abord, envoyez une demande [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) où la valeur [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) spécifie le dossier dans lequel supprimer les autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) incluent dossier : PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-295">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="ba2a5-296">Cette requête récupère le [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) pour le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-296">This request will retrieve the [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="ba2a5-297">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode **Bind** pour [supprimer des autorisations de dossier](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ba2a5-298">Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui inclut la valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le dossier a été récupéré.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-298">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="ba2a5-299">Les valeurs des éléments **FolderId** et **ParentFolderId** ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="ba2a5-300">Ensuite, utilisez l’opération **UpdateFolder** pour envoyer le **PermissionSet**mis à jour, qui n’inclut pas l' **autorisation** pour l’utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="ba2a5-301">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode **Update** pour [supprimer des autorisations de dossier](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ba2a5-302">Le serveur répond à la demande **UpdateFolder** avec un message **UpdateFolderResponse** qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que la mise à jour a réussi.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="ba2a5-303">Mise à jour des autorisations de dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="ba2a5-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-304"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="ba2a5-305">Vous pouvez également mettre à jour les autorisations de dossier pour un dossier spécifique à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="ba2a5-306">Pour mettre à jour les autorisations :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="ba2a5-307">[Supprimez les autorisations de dossier](#bk_removeewsma) pour les autorisations obsolètes, mais n’appelez pas la méthode **Update** (encore).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="ba2a5-308">[Ajoutez des autorisations de dossier pour les utilisateurs nouveaux ou modifiés](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="ba2a5-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="ba2a5-309">Appelez la méthode **Update** pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="ba2a5-310">Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une erreur **ServiceResponseException** avec la description suivante : "le jeu d’autorisations spécifié contient des userids en double".</span><span class="sxs-lookup"><span data-stu-id="ba2a5-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="ba2a5-311">Dans ce cas, supprimez les autorisations actuelles de la collection **permission** , puis ajoutez les nouvelles autorisations à la collection **permission** .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="ba2a5-312">Mise à jour des autorisations de dossier à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ba2a5-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="ba2a5-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="ba2a5-313"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="ba2a5-314">Vous pouvez également mettre à jour les autorisations de dossier pour des dossiers spécifiques à l’aide d’EWS en combinant le processus de suppression et d’ajout.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="ba2a5-315">Pour mettre à jour les autorisations :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="ba2a5-316">Récupérez les autorisations actuelles du dossier à l’aide de l’opération **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="ba2a5-317">Envoyer une liste mise à jour des autorisations à l’aide de l’opération **UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="ba2a5-318">Il s’agit des deux mêmes opérations que vous utilisez pour [activer](#bk_enableews) ou [Supprimer l’accès](#bk_removeews) à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="ba2a5-319">La seule différence réside dans le fait que lorsque vous recevez la réponse **GetFolder** , celle-ci contiendra un jeu d' **autorisations** pour user.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="ba2a5-320">Remplacez simplement cet élément d' **autorisation** existant par le nouvel élément **permission** , puis envoyez l’opération **UpdateFolder** avec la ou les nouvelles valeurs d' **autorisation** .</span><span class="sxs-lookup"><span data-stu-id="ba2a5-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="ba2a5-321">Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une valeur **ResponseCode** de **ErrorDuplicateUserIdsSpecified**.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="ba2a5-322">Dans ce cas, supprimez la valeur d’autorisation périmée pour l’utilisateur de la demande, puis renouvelez la demande.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba2a5-323">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="ba2a5-323">Next steps</span></span>

<span data-ttu-id="ba2a5-324">Une fois que vous avez accordé à un utilisateur l’autorisation d’accès à un dossier spécifique, l’utilisateur peut accéder au dossier en tant que délégué.</span><span class="sxs-lookup"><span data-stu-id="ba2a5-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="ba2a5-325">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="ba2a5-325">For more information, see:</span></span>
  
- [<span data-ttu-id="ba2a5-326">Accéder à la messagerie électronique en tant que délégué à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="ba2a5-327">Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="ba2a5-328">Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="ba2a5-329">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba2a5-329">See also</span></span>

- [<span data-ttu-id="ba2a5-330">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="ba2a5-331">Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="ba2a5-332">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba2a5-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

