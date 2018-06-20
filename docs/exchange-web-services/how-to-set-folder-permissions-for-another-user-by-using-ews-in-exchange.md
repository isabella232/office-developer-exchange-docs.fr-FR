---
title: Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754946"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="b7eda-103">Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="b7eda-104">Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7eda-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b7eda-105">Autorisations au niveau du dossier permettent aux utilisateurs d’accéder à un ou plusieurs dossiers dans la boîte aux lettres d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="b7eda-106">Autorisations de dossier sont similaires aux accès délégué, mais elles diffèrent comme suit :</span><span class="sxs-lookup"><span data-stu-id="b7eda-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="b7eda-107">Autorisations du dossier n’activez pas un utilisateur « envoyer de la part de » ou « envoyer en tant que « un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="b7eda-108">Ils autorisent l’accès aux dossiers uniquement.</span><span class="sxs-lookup"><span data-stu-id="b7eda-108">They only enable access to folders.</span></span> <span data-ttu-id="b7eda-109">Les utilisateurs peuvent créer des éléments dans les dossiers, mais ils ne peuvent pas les envoyer.</span><span class="sxs-lookup"><span data-stu-id="b7eda-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="b7eda-110">Vous pouvez définir des autorisations sur le dossier sur n’importe quel dossier dans la boîte aux lettres, mais vous ne pouvez ajouter un délégué dans les dossiers Calendrier, Contacts, boîte de réception, Journal, Notes et tâches.</span><span class="sxs-lookup"><span data-stu-id="b7eda-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="b7eda-111">Vous pouvez définir un nombre [d’autorisations sur un dossier spécifique](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="b7eda-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="b7eda-112">Lorsque vous ajoutez un délégué, vous pouvez affecter un des seuls [cinq niveaux d’autorisation](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="b7eda-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="b7eda-113">Vous pouvez définir des autorisations de dossier pour anonyme et par défaut les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="b7eda-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="b7eda-114">Vous pouvez uniquement accorder l’accès délégué à un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="b7eda-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="b7eda-115">Si vous êtes familiarisé avec les entrées de contrôle d’accès (ACE) et les listes de contrôle d’accès discrétionnaire (DACL), vous savez qu’un utilisateur peut avoir uniquement un ensemble d’autorisations pour chaque dossier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="b7eda-116">Si vous essayez d’ajouter un jeu d’autorisations pour un utilisateur et qu’ils possèdent déjà un ensemble d’autorisations, vous obtiendrez une erreur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="b7eda-117">Lorsque vous ajoutez, supprimez ou mettre à jour les autorisations sur un dossier, vous obtenez la liste DACL en cours, ajoutez ou supprimez tout ACE et puis envoyez la liste DACL mis à jour.</span><span class="sxs-lookup"><span data-stu-id="b7eda-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="b7eda-118">Vous ne pouvez pas ajouter plusieurs entrées pour le même utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="b7eda-119">Lorsque vous mettez à jour les autorisations à l’aide de l’API managée EWS, vous devez supprimer actuel ACE l’utilisateur, puis ajouter leur nouveaux ACE à la collection.</span><span class="sxs-lookup"><span data-stu-id="b7eda-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="b7eda-120">Si vous utilisez EWS, vous il suffit de remplacer l’ensemble des ACE précédente avec les nouveaux.</span><span class="sxs-lookup"><span data-stu-id="b7eda-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="b7eda-121">Si vous effectuez plusieurs modifications des autorisations à un dossier unique, vous pouvez par lot ajouts, suppressions et mises à jour, veuillez noter que vous ne pouvez pas par lots mises à jour de l’utilisateur sur plusieurs dossiers.</span><span class="sxs-lookup"><span data-stu-id="b7eda-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="b7eda-122">Un appel est nécessaire pour obtenir les autorisations sur un dossier unique et un deuxième appel est nécessaire pour mettre à jour les autorisations sur ce dossier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="b7eda-123">Lorsque vous ajoutez, supprimez ou mettre à jour les autorisations des utilisateurs, utilisez la même méthode deux appels ou opérations pour chaque tâche.</span><span class="sxs-lookup"><span data-stu-id="b7eda-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="b7eda-124">**Le tableau 1. Méthodes d’API managées et opérations EWS pour définir les autorisations de dossier**</span><span class="sxs-lookup"><span data-stu-id="b7eda-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="b7eda-125">Si vous souhaitez...</span><span class="sxs-lookup"><span data-stu-id="b7eda-125">If you want to…</span></span>|<span data-ttu-id="b7eda-126">Utilisez cette méthode d’API managées...</span><span class="sxs-lookup"><span data-stu-id="b7eda-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="b7eda-127">Utilisez cette opération EWS...</span><span class="sxs-lookup"><span data-stu-id="b7eda-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b7eda-128">Activer, supprimer ou mettre à jour les autorisations de dossier</span><span class="sxs-lookup"><span data-stu-id="b7eda-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="b7eda-129">[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7eda-129">[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="b7eda-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) suivi [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7eda-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="b7eda-131">Créez un dossier et définir les autorisations du dossier</span><span class="sxs-lookup"><span data-stu-id="b7eda-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="b7eda-132">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="b7eda-132">Folder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b7eda-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="b7eda-133">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="b7eda-134">Autorisations de dossier</span><span class="sxs-lookup"><span data-stu-id="b7eda-134">Folder permissions</span></span>
<span data-ttu-id="b7eda-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-135"></span></span>

<span data-ttu-id="b7eda-136">Vous avez quelques options en matière de définition d’autorisations de dossier sur un dossier spécifique.</span><span class="sxs-lookup"><span data-stu-id="b7eda-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="b7eda-137">Vous pouvez définir un niveau d’autorisation sur un dossier pour chaque utilisateur, qui ajoute un jeu d’autorisations individuelles prédéfinis à la liste DACL, ou vous pouvez définir des autorisations individuelles dans un dossier, mais vous ne pouvez pas combiner des.</span><span class="sxs-lookup"><span data-stu-id="b7eda-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="b7eda-138">Les autorisations spécifiques suivantes sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="b7eda-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="b7eda-139">Peut créer</span><span class="sxs-lookup"><span data-stu-id="b7eda-139">Can create</span></span>
- <span data-ttu-id="b7eda-140">Peut créer des sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="b7eda-140">Can create subfolders</span></span>    
- <span data-ttu-id="b7eda-141">Est le propriétaire du dossier</span><span class="sxs-lookup"><span data-stu-id="b7eda-141">Is folder owner</span></span>    
- <span data-ttu-id="b7eda-142">Dossier est visible</span><span class="sxs-lookup"><span data-stu-id="b7eda-142">Is folder visible</span></span>    
- <span data-ttu-id="b7eda-143">Dossier contact</span><span class="sxs-lookup"><span data-stu-id="b7eda-143">Is folder contact</span></span>    
- <span data-ttu-id="b7eda-144">Modifier des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-144">Edit items</span></span>    
- <span data-ttu-id="b7eda-145">Supprimer des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-145">Delete items</span></span>    
- <span data-ttu-id="b7eda-146">Lire des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-146">Read items</span></span>
    
<span data-ttu-id="b7eda-147">En outre, les niveaux d’autorisation suivants sont disponibles, qui définissent un sous-ensemble des autorisations spécifiques et les valeurs, comme indiqué dans le tableau 2 :</span><span class="sxs-lookup"><span data-stu-id="b7eda-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="b7eda-148">Aucun</span><span class="sxs-lookup"><span data-stu-id="b7eda-148">None</span></span>    
- <span data-ttu-id="b7eda-149">Owner</span><span class="sxs-lookup"><span data-stu-id="b7eda-149">Owner</span></span>    
- <span data-ttu-id="b7eda-150">Détenir</span><span class="sxs-lookup"><span data-stu-id="b7eda-150">PublishingEditor</span></span>    
- <span data-ttu-id="b7eda-151">Editor</span><span class="sxs-lookup"><span data-stu-id="b7eda-151">Editor</span></span>    
- <span data-ttu-id="b7eda-152">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="b7eda-152">PublishingAuthor</span></span>    
- <span data-ttu-id="b7eda-153">Auteur</span><span class="sxs-lookup"><span data-stu-id="b7eda-153">Author</span></span>    
- <span data-ttu-id="b7eda-154">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="b7eda-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="b7eda-155">Reviewer</span><span class="sxs-lookup"><span data-stu-id="b7eda-155">Reviewer</span></span>    
- <span data-ttu-id="b7eda-156">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="b7eda-156">Contributor</span></span>   
- <span data-ttu-id="b7eda-157">Personnalisé - cette valeur ne peut pas être définie par l’application.</span><span class="sxs-lookup"><span data-stu-id="b7eda-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="b7eda-158">Le serveur définit cette valeur si l’application comporte une collection personnalisée d’autorisations individuelles.</span><span class="sxs-lookup"><span data-stu-id="b7eda-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="b7eda-159">FreeBusyTimeOnly - il ne peut être définie sur dossiers de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="b7eda-160">FreeBusyTimeAndSubjectAndLocation - il ne peut être définie sur dossiers de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="b7eda-161">Le tableau suivant indique les autorisations spécifiques sont appliquées par défaut selon le niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="b7eda-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="b7eda-162">**Le tableau 2. Autorisations spécifiques à un niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="b7eda-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="b7eda-163">Niveau d’autorisation</span><span class="sxs-lookup"><span data-stu-id="b7eda-163">Permission level</span></span>|<span data-ttu-id="b7eda-164">Peut créer des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-164">Can create items</span></span>|<span data-ttu-id="b7eda-165">Peut créer des sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="b7eda-165">Can create sub folders</span></span>|<span data-ttu-id="b7eda-166">Est le propriétaire du dossier</span><span class="sxs-lookup"><span data-stu-id="b7eda-166">Is folder owner</span></span>|<span data-ttu-id="b7eda-167">Dossier est visible</span><span class="sxs-lookup"><span data-stu-id="b7eda-167">Is folder visible</span></span>|<span data-ttu-id="b7eda-168">Dossier contact</span><span class="sxs-lookup"><span data-stu-id="b7eda-168">Is folder contact</span></span>|<span data-ttu-id="b7eda-169">Modifier des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-169">Edit items</span></span>|<span data-ttu-id="b7eda-170">Supprimer des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-170">Delete items</span></span>|<span data-ttu-id="b7eda-171">Peut lire des éléments</span><span class="sxs-lookup"><span data-stu-id="b7eda-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="b7eda-172">Aucun</span><span class="sxs-lookup"><span data-stu-id="b7eda-172">None</span></span>  <br/> |<span data-ttu-id="b7eda-173">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-173">False</span></span>  <br/> |<span data-ttu-id="b7eda-174">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-174">False</span></span>  <br/> |<span data-ttu-id="b7eda-175">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-175">False</span></span>  <br/> |<span data-ttu-id="b7eda-176">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-176">False</span></span>  <br/> |<span data-ttu-id="b7eda-177">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-177">False</span></span>  <br/> |<span data-ttu-id="b7eda-178">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-178">None</span></span>  <br/> |<span data-ttu-id="b7eda-179">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-179">None</span></span>  <br/> |<span data-ttu-id="b7eda-180">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-180">None</span></span>  <br/> |
|<span data-ttu-id="b7eda-181">Owner</span><span class="sxs-lookup"><span data-stu-id="b7eda-181">Owner</span></span>  <br/> |<span data-ttu-id="b7eda-182">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-182">True</span></span>  <br/> |<span data-ttu-id="b7eda-183">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-183">True</span></span>  <br/> |<span data-ttu-id="b7eda-184">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-184">True</span></span>  <br/> |<span data-ttu-id="b7eda-185">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-185">True</span></span>  <br/> |<span data-ttu-id="b7eda-186">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-186">True</span></span>  <br/> |<span data-ttu-id="b7eda-187">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-187">All</span></span>  <br/> |<span data-ttu-id="b7eda-188">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-188">All</span></span>  <br/> |<span data-ttu-id="b7eda-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-190">Détenir</span><span class="sxs-lookup"><span data-stu-id="b7eda-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="b7eda-191">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-191">True</span></span>  <br/> |<span data-ttu-id="b7eda-192">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-192">True</span></span>  <br/> |<span data-ttu-id="b7eda-193">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-193">False</span></span>  <br/> |<span data-ttu-id="b7eda-194">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-194">True</span></span>  <br/> |<span data-ttu-id="b7eda-195">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-195">False</span></span>  <br/> |<span data-ttu-id="b7eda-196">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-196">All</span></span>  <br/> |<span data-ttu-id="b7eda-197">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-197">All</span></span>  <br/> |<span data-ttu-id="b7eda-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-199">Editor</span><span class="sxs-lookup"><span data-stu-id="b7eda-199">Editor</span></span>  <br/> |<span data-ttu-id="b7eda-200">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-200">True</span></span>  <br/> |<span data-ttu-id="b7eda-201">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-201">False</span></span>  <br/> |<span data-ttu-id="b7eda-202">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-202">False</span></span>  <br/> |<span data-ttu-id="b7eda-203">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-203">True</span></span>  <br/> |<span data-ttu-id="b7eda-204">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-204">False</span></span>  <br/> |<span data-ttu-id="b7eda-205">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-205">All</span></span>  <br/> |<span data-ttu-id="b7eda-206">Tous</span><span class="sxs-lookup"><span data-stu-id="b7eda-206">All</span></span>  <br/> |<span data-ttu-id="b7eda-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-208">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="b7eda-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="b7eda-209">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-209">True</span></span>  <br/> |<span data-ttu-id="b7eda-210">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-210">True</span></span>  <br/> |<span data-ttu-id="b7eda-211">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-211">False</span></span>  <br/> |<span data-ttu-id="b7eda-212">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-212">True</span></span>  <br/> |<span data-ttu-id="b7eda-213">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-213">False</span></span>  <br/> |<span data-ttu-id="b7eda-214">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7eda-214">Owned</span></span>  <br/> |<span data-ttu-id="b7eda-215">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7eda-215">Owned</span></span>  <br/> |<span data-ttu-id="b7eda-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-217">Auteur</span><span class="sxs-lookup"><span data-stu-id="b7eda-217">Author</span></span>  <br/> |<span data-ttu-id="b7eda-218">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-218">True</span></span>  <br/> |<span data-ttu-id="b7eda-219">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-219">False</span></span>  <br/> |<span data-ttu-id="b7eda-220">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-220">False</span></span>  <br/> |<span data-ttu-id="b7eda-221">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-221">True</span></span>  <br/> |<span data-ttu-id="b7eda-222">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-222">False</span></span>  <br/> |<span data-ttu-id="b7eda-223">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7eda-223">Owned</span></span>  <br/> |<span data-ttu-id="b7eda-224">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7eda-224">Owned</span></span>  <br/> |<span data-ttu-id="b7eda-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-226">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="b7eda-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="b7eda-227">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-227">True</span></span>  <br/> |<span data-ttu-id="b7eda-228">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-228">False</span></span>  <br/> |<span data-ttu-id="b7eda-229">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-229">False</span></span>  <br/> |<span data-ttu-id="b7eda-230">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-230">True</span></span>  <br/> |<span data-ttu-id="b7eda-231">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-231">False</span></span>  <br/> |<span data-ttu-id="b7eda-232">Aucun</span><span class="sxs-lookup"><span data-stu-id="b7eda-232">None</span></span>  <br/> |<span data-ttu-id="b7eda-233">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7eda-233">Owned</span></span>  <br/> |<span data-ttu-id="b7eda-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-235">Reviewer</span><span class="sxs-lookup"><span data-stu-id="b7eda-235">Reviewer</span></span>  <br/> |<span data-ttu-id="b7eda-236">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-236">False</span></span>  <br/> |<span data-ttu-id="b7eda-237">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-237">False</span></span>  <br/> |<span data-ttu-id="b7eda-238">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-238">False</span></span>  <br/> |<span data-ttu-id="b7eda-239">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-239">True</span></span>  <br/> |<span data-ttu-id="b7eda-240">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-240">False</span></span>  <br/> |<span data-ttu-id="b7eda-241">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-241">None</span></span>  <br/> |<span data-ttu-id="b7eda-242">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-242">None</span></span>  <br/> |<span data-ttu-id="b7eda-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b7eda-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b7eda-244">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="b7eda-244">Contributor</span></span>  <br/> |<span data-ttu-id="b7eda-245">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-245">True</span></span>  <br/> |<span data-ttu-id="b7eda-246">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-246">False</span></span>  <br/> |<span data-ttu-id="b7eda-247">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-247">False</span></span>  <br/> |<span data-ttu-id="b7eda-248">True</span><span class="sxs-lookup"><span data-stu-id="b7eda-248">True</span></span>  <br/> |<span data-ttu-id="b7eda-249">Faux</span><span class="sxs-lookup"><span data-stu-id="b7eda-249">False</span></span>  <br/> |<span data-ttu-id="b7eda-250">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-250">None</span></span>  <br/> |<span data-ttu-id="b7eda-251">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-251">None</span></span>  <br/> |<span data-ttu-id="b7eda-252">Aucune</span><span class="sxs-lookup"><span data-stu-id="b7eda-252">None</span></span>  <br/> |
   
<span data-ttu-id="b7eda-253">Si vous spécifiez un niveau d’autorisation non personnalisée dans la demande d’autorisations au niveau du dossier, vous n’avez pas besoin de spécifier les paramètres d’autorisation spécifiques.</span><span class="sxs-lookup"><span data-stu-id="b7eda-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="b7eda-254">Si vous spécifiez une autorisation lorsque vous définissez un niveau d’autorisation, une erreur **ErrorInvalidPermissionSettings** est renvoyée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b7eda-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b7eda-255">Ajout d’autorisations sur le dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b7eda-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-256"></span></span>

<span data-ttu-id="b7eda-257">L’exemple de code suivant montre comment utiliser l’API managée EWS pour :</span><span class="sxs-lookup"><span data-stu-id="b7eda-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="b7eda-258">Créer un nouvel objet [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) pour le nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-258">Create a new [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="b7eda-259">Obtenez les autorisations en cours d’un dossier à l’aide de la méthode [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b7eda-259">Get the current permissions for a folder by using the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="b7eda-260">Ajoutez la nouvelle **FolderPermissions** à la propriété [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b7eda-260">Add the new **FolderPermissions** to the [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="b7eda-261">Appelez la méthode [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les nouvelles autorisations sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-261">Call the [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="b7eda-262">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7eda-262">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="b7eda-263">La ligne de code suivante spécifie le niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="b7eda-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="b7eda-264">Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez plutôt ce code.</span><span class="sxs-lookup"><span data-stu-id="b7eda-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="b7eda-265">Lorsque vous créez un objet **FolderPermission** avec un niveau d’autorisation personnalisé, vous pouvez définir tout ou partie des [Propriétés FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) accessibles en écriture.</span><span class="sxs-lookup"><span data-stu-id="b7eda-265">You can set any or all of the writable [FolderPermission properties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="b7eda-266">Notez que le [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) n’est jamais explicitement définie sur **personnalisé** par l’application.</span><span class="sxs-lookup"><span data-stu-id="b7eda-266">Note, however, that the [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="b7eda-267">Le **FolderPermissionLevel** est définie sur personnalisé uniquement lorsque vous créez un objet **FolderPermission** et définissez des autorisations individuelles.</span><span class="sxs-lookup"><span data-stu-id="b7eda-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="b7eda-268">Ajout d’autorisations sur le dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="b7eda-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-269"></span></span>

<span data-ttu-id="b7eda-270">Les exemples de code EWS suivantes montrent comment ajouter des autorisations à un dossier spécifique à extraire les autorisations en cours et ensuite envoyer une liste des nouvelles autorisations.</span><span class="sxs-lookup"><span data-stu-id="b7eda-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="b7eda-271">La première étape consiste à envoyer une requête [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , où la valeur [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Spécifie le dossier dans lequel ajouter des autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut le dossier : PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="b7eda-271">The first step is to send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="b7eda-272">Cette requête récupère les paramètres d’autorisation pour le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="b7eda-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="b7eda-273">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Bind** pour [Ajouter des autorisations de dossier](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b7eda-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b7eda-274">Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement.</span><span class="sxs-lookup"><span data-stu-id="b7eda-274">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="b7eda-275">Les valeurs [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) et [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7eda-275">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b7eda-276">Ensuite, utilisez l’opération **UpdateFolder** pour envoyer la mise à jour [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), qui inclut l' [autorisation](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) pour le nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="b7eda-277">Notez que, y compris l’élément [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) pour le dossier respectif dans l’opération [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) remplacera tous les paramètres d’autorisation sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-277">Note that including the [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="b7eda-278">De même, y compris l’option [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) de l’opération **UpdateFolder** supprime également tous les paramètres d’autorisation sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-278">Likewise, including the [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="b7eda-279">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Update** pour [Ajouter des autorisations de dossier](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b7eda-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b7eda-280">La ligne de code suivante spécifie le niveau d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="b7eda-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="b7eda-281">Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez plutôt ce code.</span><span class="sxs-lookup"><span data-stu-id="b7eda-281">If you want to use the custom permission level, use this code instead.</span></span>
  
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

<span data-ttu-id="b7eda-282">Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été correctement mis à jour.</span><span class="sxs-lookup"><span data-stu-id="b7eda-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b7eda-283">Suppression des autorisations de dossiers à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b7eda-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-284"></span></span>

<span data-ttu-id="b7eda-285">L’exemple de code suivant montre comment utiliser l’API managée EWS pour supprimer toutes les autorisations utilisateur sur un dossier spécifique, à l’exception de par défaut et les autorisations anonymes, à :</span><span class="sxs-lookup"><span data-stu-id="b7eda-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="b7eda-286">Obtenir les autorisations en cours d’un dossier à l’aide de la méthode **Bind** .</span><span class="sxs-lookup"><span data-stu-id="b7eda-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="b7eda-287">Parcourir la collection **d’autorisations** et suppression des autorisations pour des utilisateurs individuels.</span><span class="sxs-lookup"><span data-stu-id="b7eda-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="b7eda-288">L’appel de la méthode **Update** pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="b7eda-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="b7eda-289">Cet exemple supprime toutes les autorisations utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="b7eda-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="b7eda-290">Si vous souhaitez modifier cet exemple pour supprimer des autorisations uniquement pour un utilisateur spécifique, modifiez la ligne suivante de code pour identifier le nom complet ou l’adresse SMTP de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="b7eda-291">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7eda-291">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="b7eda-292">Suppression des autorisations de dossiers à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="b7eda-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-293"></span></span>

<span data-ttu-id="b7eda-294">Les exemples de code EWS suivants montrent comment supprimer toutes les autorisations utilisateur sur un dossier spécifique, sauf pour les autorisations anonymes et par défaut.</span><span class="sxs-lookup"><span data-stu-id="b7eda-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="b7eda-295">Tout d’abord, envoyez une requête de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) où la valeur [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Spécifie le dossier dans lequel supprimer les autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut le dossier : PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="b7eda-295">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="b7eda-296">Cette requête extrait le [jeu d’autorisations](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) pour le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="b7eda-296">This request will retrieve the [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="b7eda-297">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Bind** pour [Supprimer les autorisations du dossier](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="b7eda-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b7eda-298">Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement.</span><span class="sxs-lookup"><span data-stu-id="b7eda-298">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="b7eda-299">Les valeurs des éléments **FolderId** et **ParentFolderId** ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b7eda-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b7eda-300">Ensuite, utilisez l’opération **UpdateFolder** pour envoyer la mise à jour **PermissionSet**, qui n’inclut pas l' **autorisation** de l’utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="b7eda-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="b7eda-301">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode de **mise à jour** pour [Supprimer les autorisations du dossier](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="b7eda-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b7eda-302">Le serveur répond à la demande **UpdateFolder** avec un message **UpdateFolderResponse** qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la mise à jour a réussi.</span><span class="sxs-lookup"><span data-stu-id="b7eda-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b7eda-303">Mise à jour des autorisations de dossiers à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b7eda-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-304"></span></span>

<span data-ttu-id="b7eda-305">Vous pouvez également mettre à jour les autorisations du dossier pour un dossier spécifique à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="b7eda-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="b7eda-306">Pour mettre à jour les autorisations :</span><span class="sxs-lookup"><span data-stu-id="b7eda-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="b7eda-307">[Supprimer les autorisations de dossier](#bk_removeewsma) pour les autorisations obsolètes, mais vous n’appelez pas la méthode de **mise à jour** (encore).</span><span class="sxs-lookup"><span data-stu-id="b7eda-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="b7eda-308">[Ajouter des autorisations de dossier pour les utilisateurs nouveaux ou modifiés](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b7eda-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="b7eda-309">Appelez la méthode **Update** pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="b7eda-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="b7eda-310">Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une erreur **ServiceResponseException** avec la description suivante : « le jeu d’autorisations spécifié contient les ID utilisateur en double ».</span><span class="sxs-lookup"><span data-stu-id="b7eda-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="b7eda-311">Dans ce cas, supprimez les autorisations en cours de la collection **Permission** , puis ajoutez les nouvelles autorisations à la collection **Permission** .</span><span class="sxs-lookup"><span data-stu-id="b7eda-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="b7eda-312">Mise à jour des autorisations de dossiers à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b7eda-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="b7eda-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="b7eda-313"></span></span>

<span data-ttu-id="b7eda-314">Vous pouvez également mettre à jour des autorisations de dossiers pour des dossiers spécifiques à l’aide de EWS en combinant le processus de suppression et d’ajout.</span><span class="sxs-lookup"><span data-stu-id="b7eda-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="b7eda-315">Pour mettre à jour les autorisations :</span><span class="sxs-lookup"><span data-stu-id="b7eda-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="b7eda-316">Récupérer les autorisations du dossier en cours à l’aide de l’opération **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="b7eda-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="b7eda-317">Envoyer une liste mise à jour des autorisations à l’aide de l’opération **UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="b7eda-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="b7eda-318">Voici les deux opérations même que vous utilisez pour [Activer](#bk_enableews) ou [Supprimer l’accès](#bk_removeews) à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="b7eda-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="b7eda-319">La seule différence est que lorsque vous recevez la réponse **GetFolder** , il contient un jeu d' **autorisations** pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7eda-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="b7eda-320">Remplacez simplement cet élément **d’autorisation** existant par le nouvel élément **d’autorisation** , puis envoyer l’opération **UpdateFolder** avec la nouvelle valeur **d’autorisation** ou les valeurs.</span><span class="sxs-lookup"><span data-stu-id="b7eda-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="b7eda-321">Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une valeur **ResponseCode** **ErrorDuplicateUserIdsSpecified**.</span><span class="sxs-lookup"><span data-stu-id="b7eda-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="b7eda-322">Dans ce cas, supprimez la valeur d’autorisation obsolète pour l’utilisateur de la demande et réessayez d’exécuter la requête.</span><span class="sxs-lookup"><span data-stu-id="b7eda-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b7eda-323">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="b7eda-323">Next steps</span></span>

<span data-ttu-id="b7eda-324">Une fois que vous autorisez un utilisateur à un dossier spécifique, l’utilisateur peut accéder au dossier en tant que délégué.</span><span class="sxs-lookup"><span data-stu-id="b7eda-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="b7eda-325">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="b7eda-325">For more information, see:</span></span>
  
- [<span data-ttu-id="b7eda-326">Accéder à la messagerie en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b7eda-327">Accéder à un calendrier en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b7eda-328">Contacts Access en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="b7eda-329">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7eda-329">See also</span></span>

- [<span data-ttu-id="b7eda-330">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="b7eda-331">Ajouter et supprimer des délégués à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="b7eda-332">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7eda-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

