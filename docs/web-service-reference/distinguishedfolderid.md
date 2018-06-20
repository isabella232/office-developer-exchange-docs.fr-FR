---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: L’élément DistinguishedFolderId identifie les dossiers qui peuvent être référencés par un nom. Si vous n’utilisez pas cet élément, vous devez utiliser l’élément FolderId pour identifier un dossier.
ms.openlocfilehash: 834166be3d882fa8c0533cfcc2999600430b82ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756018"
---
# <a name="distinguishedfolderid"></a><span data-ttu-id="58b91-104">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-104">DistinguishedFolderId</span></span>

<span data-ttu-id="58b91-105">L’élément **DistinguishedFolderId** identifie les dossiers qui peuvent être référencés par un nom.</span><span class="sxs-lookup"><span data-stu-id="58b91-105">The **DistinguishedFolderId** element identifies folders that can be referenced by name.</span></span> <span data-ttu-id="58b91-106">Si vous n’utilisez pas cet élément, vous devez utiliser l’élément [FolderId](folderid.md) pour identifier un dossier.</span><span class="sxs-lookup"><span data-stu-id="58b91-106">If you do not use this element, you must use the [FolderId](folderid.md) element to identify a folder.</span></span> 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 <span data-ttu-id="58b91-107">**DistinguishedFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="58b91-107">**DistinguishedFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58b91-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="58b91-108">Attributes and elements</span></span>

<span data-ttu-id="58b91-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="58b91-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58b91-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="58b91-110">Attributes</span></span>

|<span data-ttu-id="58b91-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="58b91-111">**Attribute**</span></span>|<span data-ttu-id="58b91-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="58b91-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="58b91-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="58b91-113">**Id**</span></span> <br/> |<span data-ttu-id="58b91-114">Contient une chaîne qui identifie un dossier par défaut.</span><span class="sxs-lookup"><span data-stu-id="58b91-114">Contains a string that identifies a default folder.</span></span> <span data-ttu-id="58b91-115">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="58b91-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="58b91-116">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="58b91-116">**ChangeKey**</span></span> <br/> |<span data-ttu-id="58b91-117">Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut **Id** .</span><span class="sxs-lookup"><span data-stu-id="58b91-117">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="58b91-118">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="58b91-118">This attribute is optional.</span></span> <span data-ttu-id="58b91-119">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="58b91-119">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
#### <a name="id-attribute-values"></a><span data-ttu-id="58b91-120">Valeurs d’attribut ID</span><span class="sxs-lookup"><span data-stu-id="58b91-120">Id attribute values</span></span>

|<span data-ttu-id="58b91-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="58b91-121">**Value**</span></span>|<span data-ttu-id="58b91-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="58b91-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="58b91-123">calendrier</span><span class="sxs-lookup"><span data-stu-id="58b91-123">calendar</span></span>  <br/> |<span data-ttu-id="58b91-124">Représente le dossier calendrier.</span><span class="sxs-lookup"><span data-stu-id="58b91-124">Represents the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-125">contacts</span><span class="sxs-lookup"><span data-stu-id="58b91-125">contacts</span></span>  <br/> |<span data-ttu-id="58b91-126">Représente le dossier Contacts.</span><span class="sxs-lookup"><span data-stu-id="58b91-126">Represents the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-127">deleteditems</span><span class="sxs-lookup"><span data-stu-id="58b91-127">deleteditems</span></span>  <br/> |<span data-ttu-id="58b91-128">Représente le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="58b91-128">Represents the Deleted Items folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-129">brouillons</span><span class="sxs-lookup"><span data-stu-id="58b91-129">drafts</span></span>  <br/> |<span data-ttu-id="58b91-130">Représente le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="58b91-130">Represents the Drafts folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-131">boîte de réception</span><span class="sxs-lookup"><span data-stu-id="58b91-131">inbox</span></span>  <br/> |<span data-ttu-id="58b91-132">Représente le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="58b91-132">Represents the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-133">journal</span><span class="sxs-lookup"><span data-stu-id="58b91-133">journal</span></span>  <br/> |<span data-ttu-id="58b91-134">Représente le dossier Journal.</span><span class="sxs-lookup"><span data-stu-id="58b91-134">Represents the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-135">notes</span><span class="sxs-lookup"><span data-stu-id="58b91-135">notes</span></span>  <br/> |<span data-ttu-id="58b91-136">Représente le dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="58b91-136">Represents the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-137">la boîte d’envoi</span><span class="sxs-lookup"><span data-stu-id="58b91-137">outbox</span></span>  <br/> |<span data-ttu-id="58b91-138">Représente le dossier boîte d’envoi.</span><span class="sxs-lookup"><span data-stu-id="58b91-138">Represents the Outbox folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-139">éléments envoyés</span><span class="sxs-lookup"><span data-stu-id="58b91-139">sentitems</span></span>  <br/> |<span data-ttu-id="58b91-140">Représente le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="58b91-140">Represents the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-141">tasks</span><span class="sxs-lookup"><span data-stu-id="58b91-141">tasks</span></span>  <br/> |<span data-ttu-id="58b91-142">Représente le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="58b91-142">Represents the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-143">msgfolderroot</span><span class="sxs-lookup"><span data-stu-id="58b91-143">msgfolderroot</span></span>  <br/> |<span data-ttu-id="58b91-144">Représente la racine du dossier du message.</span><span class="sxs-lookup"><span data-stu-id="58b91-144">Represents the message folder root.</span></span>  <br/> |
|<span data-ttu-id="58b91-145">root</span><span class="sxs-lookup"><span data-stu-id="58b91-145">root</span></span>  <br/> |<span data-ttu-id="58b91-146">Représente la racine de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="58b91-146">Represents the root of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="58b91-147">junkemail</span><span class="sxs-lookup"><span data-stu-id="58b91-147">junkemail</span></span>  <br/> |<span data-ttu-id="58b91-148">Représente le dossier courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="58b91-148">Represents the Junk Email folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-149">SearchFolders</span><span class="sxs-lookup"><span data-stu-id="58b91-149">searchfolders</span></span>  <br/> |<span data-ttu-id="58b91-150">Représente le dossier de dossiers de recherche.</span><span class="sxs-lookup"><span data-stu-id="58b91-150">Represents the Search Folders folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-151">messagerie vocale</span><span class="sxs-lookup"><span data-stu-id="58b91-151">voicemail</span></span>  <br/> |<span data-ttu-id="58b91-152">Représente le dossier de messagerie vocale.</span><span class="sxs-lookup"><span data-stu-id="58b91-152">Represents the Voice Mail folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-153">recoverableitemsroot</span><span class="sxs-lookup"><span data-stu-id="58b91-153">recoverableitemsroot</span></span>  <br/> |<span data-ttu-id="58b91-154">Représente la benne de dossier racine.</span><span class="sxs-lookup"><span data-stu-id="58b91-154">Represents the dumpster root folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-155">recoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="58b91-155">recoverableitemsdeletions</span></span>  <br/> |<span data-ttu-id="58b91-156">Représente la benne de dossier de suppressions.</span><span class="sxs-lookup"><span data-stu-id="58b91-156">Represents the dumpster deletions folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-157">recoverableitemsversions</span><span class="sxs-lookup"><span data-stu-id="58b91-157">recoverableitemsversions</span></span>  <br/> |<span data-ttu-id="58b91-158">Représente la benne de dossier de versions.</span><span class="sxs-lookup"><span data-stu-id="58b91-158">Represents the dumpster versions folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-159">recoverableitemspurges</span><span class="sxs-lookup"><span data-stu-id="58b91-159">recoverableitemspurges</span></span>  <br/> |<span data-ttu-id="58b91-160">Représente la benne de purge du dossier.</span><span class="sxs-lookup"><span data-stu-id="58b91-160">Represents the dumpster purges folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-161">archiveroot</span><span class="sxs-lookup"><span data-stu-id="58b91-161">archiveroot</span></span>  <br/> |<span data-ttu-id="58b91-162">Représente le dossier racine d’archivage.</span><span class="sxs-lookup"><span data-stu-id="58b91-162">Represents the root archive folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-163">archivemsgfolderroot</span><span class="sxs-lookup"><span data-stu-id="58b91-163">archivemsgfolderroot</span></span>  <br/> |<span data-ttu-id="58b91-164">Représente le dossier messages d’archivage racine.</span><span class="sxs-lookup"><span data-stu-id="58b91-164">Represents the root archive message folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-165">archivedeleteditems</span><span class="sxs-lookup"><span data-stu-id="58b91-165">archivedeleteditems</span></span>  <br/> |<span data-ttu-id="58b91-166">Représente le dossier d’éléments supprimés des archives.</span><span class="sxs-lookup"><span data-stu-id="58b91-166">Represents the archive deleted items folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-167">archiveinbox</span><span class="sxs-lookup"><span data-stu-id="58b91-167">archiveinbox</span></span>  <br/> |<span data-ttu-id="58b91-168">Représente le dossier boîte de réception de l’archive.</span><span class="sxs-lookup"><span data-stu-id="58b91-168">Represents the archive Inbox folder.</span></span> <span data-ttu-id="58b91-169">Versions d’Exchange commençant par le numéro de build 15.00.0913.09 incluent cette valeur.</span><span class="sxs-lookup"><span data-stu-id="58b91-169">Versions of Exchange starting with build number 15.00.0913.09 include this value.</span></span>  <br/> |
|<span data-ttu-id="58b91-170">archiverecoverableitemsroot</span><span class="sxs-lookup"><span data-stu-id="58b91-170">archiverecoverableitemsroot</span></span>  <br/> |<span data-ttu-id="58b91-171">Représente le dossier racine d’archivage éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="58b91-171">Represents the archive recoverable items root folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-172">archiverecoverableitemsdeletions</span><span class="sxs-lookup"><span data-stu-id="58b91-172">archiverecoverableitemsdeletions</span></span>  <br/> |<span data-ttu-id="58b91-173">Représente le dossier de suppressions d’éléments récupérables archive.</span><span class="sxs-lookup"><span data-stu-id="58b91-173">Represents the archive recoverable items deletions folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-174">archiverecoverableitemsversions</span><span class="sxs-lookup"><span data-stu-id="58b91-174">archiverecoverableitemsversions</span></span>  <br/> |<span data-ttu-id="58b91-175">Représente le dossier de versions d’éléments récupérables archive.</span><span class="sxs-lookup"><span data-stu-id="58b91-175">Represents the archive recoverable items versions folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-176">archiverecoverableitemspurges</span><span class="sxs-lookup"><span data-stu-id="58b91-176">archiverecoverableitemspurges</span></span>  <br/> |<span data-ttu-id="58b91-177">Représente le dossier de purge archive les éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="58b91-177">Represents the archive recoverable items purges folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-178">syncissues</span><span class="sxs-lookup"><span data-stu-id="58b91-178">syncissues</span></span>  <br/> |<span data-ttu-id="58b91-179">Représente le dossier problèmes de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="58b91-179">Represents the sync issues folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-180">conflits</span><span class="sxs-lookup"><span data-stu-id="58b91-180">conflicts</span></span>  <br/> |<span data-ttu-id="58b91-181">Représente le dossier conflits.</span><span class="sxs-lookup"><span data-stu-id="58b91-181">Represents the conflicts folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-182">localfailures</span><span class="sxs-lookup"><span data-stu-id="58b91-182">localfailures</span></span>  <br/> |<span data-ttu-id="58b91-183">Représente le dossier Pannes locales.</span><span class="sxs-lookup"><span data-stu-id="58b91-183">Represents the local failures folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-184">serverfailures</span><span class="sxs-lookup"><span data-stu-id="58b91-184">serverfailures</span></span>  <br/> |<span data-ttu-id="58b91-185">Représente le dossier échecs du serveur.</span><span class="sxs-lookup"><span data-stu-id="58b91-185">Represents the server failures folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-186">recipientcache</span><span class="sxs-lookup"><span data-stu-id="58b91-186">recipientcache</span></span>  <br/> |<span data-ttu-id="58b91-187">Représente le dossier de cache de destinataires.</span><span class="sxs-lookup"><span data-stu-id="58b91-187">Represents the recipient cache folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-188">QuickContacts</span><span class="sxs-lookup"><span data-stu-id="58b91-188">quickcontacts</span></span>  <br/> |<span data-ttu-id="58b91-189">Représente le dossier contacts rapides.</span><span class="sxs-lookup"><span data-stu-id="58b91-189">Represents the quick contacts folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-190">conversationhistory</span><span class="sxs-lookup"><span data-stu-id="58b91-190">conversationhistory</span></span>  <br/> |<span data-ttu-id="58b91-191">Représente le dossier historique des conversations.</span><span class="sxs-lookup"><span data-stu-id="58b91-191">Represents the conversation history folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-192">adminauditlogs</span><span class="sxs-lookup"><span data-stu-id="58b91-192">adminauditlogs</span></span>  <br/> |<span data-ttu-id="58b91-193">Représente le dossier des journaux d’audit d’administration.</span><span class="sxs-lookup"><span data-stu-id="58b91-193">Represents the admin audit logs folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-194">todosearch</span><span class="sxs-lookup"><span data-stu-id="58b91-194">todosearch</span></span>  <br/> |<span data-ttu-id="58b91-195">Représente le dossier de recherche des tâches.</span><span class="sxs-lookup"><span data-stu-id="58b91-195">Represents the todo search folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-196">mescontacts</span><span class="sxs-lookup"><span data-stu-id="58b91-196">mycontacts</span></span>  <br/> |<span data-ttu-id="58b91-197">Représente le dossier Mes Contacts.</span><span class="sxs-lookup"><span data-stu-id="58b91-197">Represents the My Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-198">répertoire</span><span class="sxs-lookup"><span data-stu-id="58b91-198">directory</span></span>  <br/> |<span data-ttu-id="58b91-199">Représente le dossier de répertoire.</span><span class="sxs-lookup"><span data-stu-id="58b91-199">Represents the directory folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-200">imcontactlist</span><span class="sxs-lookup"><span data-stu-id="58b91-200">imcontactlist</span></span>  <br/> |<span data-ttu-id="58b91-201">Représente le dossier de liste de contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="58b91-201">Represents the IM contact list folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-202">peopleconnect</span><span class="sxs-lookup"><span data-stu-id="58b91-202">peopleconnect</span></span>  <br/> |<span data-ttu-id="58b91-203">Représente les personnes connecter le dossier.</span><span class="sxs-lookup"><span data-stu-id="58b91-203">Represents the people connect folder.</span></span>  <br/> |
|<span data-ttu-id="58b91-204">favoris</span><span class="sxs-lookup"><span data-stu-id="58b91-204">favorites</span></span>  <br/> |<span data-ttu-id="58b91-205">Représente le dossier Favoris.</span><span class="sxs-lookup"><span data-stu-id="58b91-205">Represents the Favorites folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="58b91-206">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="58b91-206">Child elements</span></span>

|<span data-ttu-id="58b91-207">**Élément**</span><span class="sxs-lookup"><span data-stu-id="58b91-207">**Element**</span></span>|<span data-ttu-id="58b91-208">**Description**</span><span class="sxs-lookup"><span data-stu-id="58b91-208">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58b91-209">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="58b91-209">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="58b91-210">Identifie une adresse SMTP principale.</span><span class="sxs-lookup"><span data-stu-id="58b91-210">Identifies a primary SMTP address.</span></span> <span data-ttu-id="58b91-211">Adresses proxy ne sont pas autorisés.</span><span class="sxs-lookup"><span data-stu-id="58b91-211">Proxy addresses are not allowed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58b91-212">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="58b91-212">Parent elements</span></span>

|<span data-ttu-id="58b91-213">**Élément**</span><span class="sxs-lookup"><span data-stu-id="58b91-213">**Element**</span></span>|<span data-ttu-id="58b91-214">**Description**</span><span class="sxs-lookup"><span data-stu-id="58b91-214">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58b91-215">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-215">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="58b91-216">Indique le dossier qui est destiné aux actions de conversation qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="58b91-216">Indicates the folder that is targeted for conversation actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="58b91-217">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-217">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="58b91-218">Indique le dossier de destination de copie et déplacer les actions de conversation.</span><span class="sxs-lookup"><span data-stu-id="58b91-218">Indicates the destination folder for copy and move conversation actions.</span></span>  <br/> |
|[<span data-ttu-id="58b91-219">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="58b91-219">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="58b91-220">Identifie le dossier dans lequel un nouveau dossier ou un élément est créé.</span><span class="sxs-lookup"><span data-stu-id="58b91-220">Identifies the folder in which a new folder or item is created.</span></span>  <br/><br/><span data-ttu-id="58b91-221">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="58b91-221">The following are the XPath expressions to this element:</span></span><br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="58b91-222">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="58b91-222">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="58b91-223">Identifie les dossiers de recherche de l' [opération FindItem](finditem-operation.md) et l' [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="58b91-223">Identifies folders to search for the [FindItem operation](finditem-operation.md) and the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="58b91-224">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="58b91-224">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="58b91-225">Représente la collection de dossiers portera pour déterminer le contenu d’un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="58b91-225">Represents the collection of folders that will be searched to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="58b91-226">FolderIds</span><span class="sxs-lookup"><span data-stu-id="58b91-226">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="58b91-227">Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements.</span><span class="sxs-lookup"><span data-stu-id="58b91-227">Contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="58b91-228">FolderChange</span><span class="sxs-lookup"><span data-stu-id="58b91-228">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="58b91-229">Représente une collection des modifications à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="58b91-229">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <br/><span data-ttu-id="58b91-230">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="58b91-230">The following is the XPath expression to this element:</span></span><br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[<span data-ttu-id="58b91-231">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-231">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="58b91-232">Représente le dossier de destination pour un dossier ou un élément copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="58b91-232">Represents the destination folder for a copied or moved item or folder.</span></span><br/><br/><span data-ttu-id="58b91-233">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="58b91-233">The following are the XPath expressions to this element:</span></span><br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="58b91-234">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-234">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="58b91-235">Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="58b91-235">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span><br/><br/><span data-ttu-id="58b91-236">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="58b91-236">The following are the XPath expressions to this element:</span></span><br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="58b91-237">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="58b91-237">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="58b91-238">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="58b91-238">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="58b91-239">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="58b91-239">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="58b91-240">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="58b91-240">Represents the name of a user configuration object.</span></span> <span data-ttu-id="58b91-241">Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="58b91-241">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="58b91-242">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="58b91-242">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="58b91-243">Représente l’ID du dossier e-mail éléments vont être copiés dans.</span><span class="sxs-lookup"><span data-stu-id="58b91-243">Represents the ID of the folder that email items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="58b91-244">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="58b91-244">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="58b91-245">Représente l’ID du dossier éléments seront déplacées vers e-mail.</span><span class="sxs-lookup"><span data-stu-id="58b91-245">Represents the ID of the folder that email items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58b91-246">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="58b91-246">Text value</span></span>

<span data-ttu-id="58b91-247">Aucun.</span><span class="sxs-lookup"><span data-stu-id="58b91-247">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58b91-248">Remarques</span><span class="sxs-lookup"><span data-stu-id="58b91-248">Remarks</span></span>

<span data-ttu-id="58b91-249">Un **DistinguishedFolderId** résout un **FolderId**.</span><span class="sxs-lookup"><span data-stu-id="58b91-249">A **DistinguishedFolderId** resolves to a **FolderId**.</span></span> 
  
<span data-ttu-id="58b91-250">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="58b91-250">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58b91-251">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="58b91-251">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58b91-252">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="58b91-252">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58b91-253">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="58b91-253">Schema Name</span></span>  <br/> |<span data-ttu-id="58b91-254">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="58b91-254">Types schema</span></span>  <br/> |
|<span data-ttu-id="58b91-255">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="58b91-255">Validation File</span></span>  <br/> |<span data-ttu-id="58b91-256">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="58b91-256">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58b91-257">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="58b91-257">Can be Empty</span></span>  <br/> |<span data-ttu-id="58b91-258">False</span><span class="sxs-lookup"><span data-stu-id="58b91-258">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58b91-259">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="58b91-259">See also</span></span>

- [<span data-ttu-id="58b91-260">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="58b91-260">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="58b91-261">Création de dossiers (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="58b91-261">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)
