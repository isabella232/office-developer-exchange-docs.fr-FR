---
title: Fonctionnalité EWS dans les versions de produit Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS implémente de nouvelles fonctionnalités dans les nouvelles versions du produit. Utilisez les informations de cet article pour déterminer si la version d’Exchange que vous ciblez prend en charge les données ou le besoin d’accéder à des fonctionnalités.
ms.openlocfilehash: 6b676781f25eeeb90fd9ab075fbe63198766bd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754773"
---
# <a name="ews-functionality-in-exchange-product-versions"></a><span data-ttu-id="10ac7-104">Fonctionnalité EWS dans les versions de produit Exchange</span><span class="sxs-lookup"><span data-stu-id="10ac7-104">EWS functionality in Exchange product versions</span></span>

<span data-ttu-id="10ac7-105">EWS implémente de nouvelles fonctionnalités dans les nouvelles versions du produit.</span><span class="sxs-lookup"><span data-stu-id="10ac7-105">EWS implements new functionality in new product releases.</span></span> <span data-ttu-id="10ac7-106">Utilisez les informations de cet article pour déterminer si la version d’Exchange que vous ciblez prend en charge les données ou le besoin d’accéder à des fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="10ac7-106">Use the information in this article to determine whether the version of Exchange you're targeting includes support for the data or features you need access to.</span></span> 
  
<span data-ttu-id="10ac7-107">Le tableau suivant répertorie les versions d’Exchange incluant les EWS et les principales fonctionnalités qui ont été introduites dans chaque version.</span><span class="sxs-lookup"><span data-stu-id="10ac7-107">The following table lists the versions of Exchange that include EWS and the major features that were introduced in each version.</span></span>
  
## <a name="ews-features-by-product-version"></a><span data-ttu-id="10ac7-108">Fonctionnalités EWS par version de produit</span><span class="sxs-lookup"><span data-stu-id="10ac7-108">EWS features by product version</span></span>

|<span data-ttu-id="10ac7-109">**Version du produit**</span><span class="sxs-lookup"><span data-stu-id="10ac7-109">**Product version**</span></span>|<span data-ttu-id="10ac7-110">**Fonctionnalités**</span><span class="sxs-lookup"><span data-stu-id="10ac7-110">**Features**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10ac7-111">Office 365 et Exchange Online</span><span class="sxs-lookup"><span data-stu-id="10ac7-111">Office 365 and Exchange Online</span></span> |<span data-ttu-id="10ac7-112">Inclut toutes les fonctionnalités dans la version actuelle d’Exchange, en plus de ces nouvelles fonctionnalités sont ajoutées pour les clients en ligne.</span><span class="sxs-lookup"><span data-stu-id="10ac7-112">Includes all the features in the current version of Exchange in addition to any new features that are added for online clients.</span></span>  |
|<span data-ttu-id="10ac7-113">Exchange 2013 SP1</span><span class="sxs-lookup"><span data-stu-id="10ac7-113">Exchange 2013 SP1</span></span> | <span data-ttu-id="10ac7-114">Inclut toutes les fonctionnalités introduites dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="10ac7-114">Includes all features introduced in Exchange 2013.</span></span> <span data-ttu-id="10ac7-115">Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-115">The following features were introduced in Exchange 2013 SP1:</span></span><ul><li><span data-ttu-id="10ac7-116">Confirmations de lecture peuvent maintenant être suspendues pour les mises à jour et suppressions.</span><span class="sxs-lookup"><span data-stu-id="10ac7-116">Read receipts can now be suspended for updates and deletions.</span></span></li><li><span data-ttu-id="10ac7-117">Vous pouvez obtenir des informations d’approbation [modérés transport](http://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="10ac7-117">You can get [moderated transport](http://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) approval information.</span></span></li><li><span data-ttu-id="10ac7-118">Réponses de vote peut être affiché.</span><span class="sxs-lookup"><span data-stu-id="10ac7-118">Voting responses can be viewed.</span></span></li><li><span data-ttu-id="10ac7-119">La méthode [SetHoldOnMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) et [SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) opération acceptent tous les paramètres dans un seul objet.</span><span class="sxs-lookup"><span data-stu-id="10ac7-119">The [SetHoldOnMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) method and [SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) operation accept all the parameters in a single object.</span></span></li><li><span data-ttu-id="10ac7-120">recherches de découverte électronique peuvent spécifier une langue pour les requêtes de recherche et un format spécifique à la culture pour les plages de dates.</span><span class="sxs-lookup"><span data-stu-id="10ac7-120">eDiscovery searches can specify a language for search queries and a culture-specific format for date ranges.</span></span></li><li><span data-ttu-id="10ac7-121">L’objet [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) permettre maintenant accéder les objets [StreamingSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="10ac7-121">The [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) object can now access the [StreamingSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) objects.</span></span></li><li><span data-ttu-id="10ac7-122">Conversations ont un paramètre pour indiquer s’ils contiennent des messages électroniques qui sont protégés par IRM.</span><span class="sxs-lookup"><span data-stu-id="10ac7-122">Conversations have a setting to indicate whether they contain email messages that are protected by IRM.</span></span></li><li><span data-ttu-id="10ac7-123">Les participants aux réunions, vous pouvez proposer de début et de fin des heures pour les réunions et les inclure dans leur réponse à une réunion.</span><span class="sxs-lookup"><span data-stu-id="10ac7-123">Meeting attendees can propose new start and end times for meetings and include them in their meeting response.</span></span></li><li><span data-ttu-id="10ac7-124">La méthode SOAP Autodiscover [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) maintenant, renvoie le [GroupingInformation](http://msdn.microsoft.com/EN-US/library/office/dn529149%28v=exchg.150%29.aspx) qui est utilisé conserve les affinités pour un abonnement aux événements plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="10ac7-124">The SOAP Autodiscover [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method now returns the [GroupingInformation](http://msdn.microsoft.com/EN-US/library/office/dn529149%28v=exchg.150%29.aspx) setting that is used maintain affinity for a multiple mailbox event subscription.</span></span></li></ul> |
|<span data-ttu-id="10ac7-125">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="10ac7-125">Exchange 2013</span></span>  | <span data-ttu-id="10ac7-126">Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP2.</span><span class="sxs-lookup"><span data-stu-id="10ac7-126">Includes all features introduced in Exchange 2010 SP2.</span></span> <span data-ttu-id="10ac7-127">Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-127">The following features were introduced in Exchange 2013:</span></span>  <ul><li>  <span data-ttu-id="10ac7-128">L’archivage</span><span class="sxs-lookup"><span data-stu-id="10ac7-128">Archiving</span></span></li><li><span data-ttu-id="10ac7-129">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="10ac7-129">eDiscovery</span></span></li><li><span data-ttu-id="10ac7-130">Personnage</span><span class="sxs-lookup"><span data-stu-id="10ac7-130">Personas</span></span></li><li><span data-ttu-id="10ac7-131">Stratégies de rétention</span><span class="sxs-lookup"><span data-stu-id="10ac7-131">Retention policies</span></span></li><li><span data-ttu-id="10ac7-132">Magasin de contacts unifié</span><span class="sxs-lookup"><span data-stu-id="10ac7-132">Unified Contact Store</span></span></li><li><span data-ttu-id="10ac7-133">Photos de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="10ac7-133">User photos</span></span></li></ul> |
|<span data-ttu-id="10ac7-134">Exchange 2010 SP2</span><span class="sxs-lookup"><span data-stu-id="10ac7-134">Exchange 2010 SP2</span></span>  | <span data-ttu-id="10ac7-135">Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1.</span><span class="sxs-lookup"><span data-stu-id="10ac7-135">Includes all the features introduced in Exchange 2010 SP1.</span></span> <span data-ttu-id="10ac7-136">Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-136">The following features were introduced in Exchange 2010 SP2:</span></span>  <ul><li>  <span data-ttu-id="10ac7-137">Obtenir l’Expiration du mot de passe</span><span class="sxs-lookup"><span data-stu-id="10ac7-137">Get Password Expiration</span></span></li><li><span data-ttu-id="10ac7-138">Précision DateTime</span><span class="sxs-lookup"><span data-stu-id="10ac7-138">DateTime precision</span></span></li><li><span data-ttu-id="10ac7-139">Identificateurs de propriété mis à jour pour les contacts</span><span class="sxs-lookup"><span data-stu-id="10ac7-139">Updated property identifiers for contacts</span></span></li><li><span data-ttu-id="10ac7-140">Nouveaux scénarios de l’emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="10ac7-140">New impersonation scenarios</span></span></li></ul> |
|<span data-ttu-id="10ac7-141">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="10ac7-141">Exchange 2010 SP1</span></span>  | <span data-ttu-id="10ac7-142">Inclut toutes les fonctionnalités introduites dans Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="10ac7-142">Includes all the features introduced in Exchange 2010.</span></span> <span data-ttu-id="10ac7-143">Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-143">The following features were introduced in Exchange 2010 SP1:</span></span>  <ul><li>  <span data-ttu-id="10ac7-144">Créer, récupérer et modifier des règles de boîte de réception</span><span class="sxs-lookup"><span data-stu-id="10ac7-144">Create, retrieve and modify Inbox rules</span></span></li><li><span data-ttu-id="10ac7-145">Accès par programme aux boîtes aux lettres d’Archive</span><span class="sxs-lookup"><span data-stu-id="10ac7-145">Programmatic access to Archive Mailbox</span></span></li><li><span data-ttu-id="10ac7-146">Actions de conversations</span><span class="sxs-lookup"><span data-stu-id="10ac7-146">Conversations actions</span></span></li><li><span data-ttu-id="10ac7-147">Le parcours des notifications de pare-feu</span><span class="sxs-lookup"><span data-stu-id="10ac7-147">Firewall traversing notifications</span></span></li><li><span data-ttu-id="10ac7-148">Fonctionnalités d’administration améliorée</span><span class="sxs-lookup"><span data-stu-id="10ac7-148">Improved administration features</span></span></li><li><span data-ttu-id="10ac7-149">Amélioration de la prise en charge de la version mixte</span><span class="sxs-lookup"><span data-stu-id="10ac7-149">Improved mixed version support</span></span></li><li><span data-ttu-id="10ac7-150">Limitation de la prise en charge de la protection</span><span class="sxs-lookup"><span data-stu-id="10ac7-150">Throttling protection support</span></span></li><li><span data-ttu-id="10ac7-151">Contrôle d’accès application EWS</span><span class="sxs-lookup"><span data-stu-id="10ac7-151">Control of application access to EWS</span></span></li><li><span data-ttu-id="10ac7-152">Prise en charge de l’authentification de certificat client</span><span class="sxs-lookup"><span data-stu-id="10ac7-152">Client certificate authentication support</span></span></li></ul> |
|<span data-ttu-id="10ac7-153">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="10ac7-153">Exchange 2010</span></span>  | <span data-ttu-id="10ac7-154">Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="10ac7-154">Includes all features introduced in Exchange 2007 SP1.</span></span> <span data-ttu-id="10ac7-155">Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2010 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-155">The following features were introduced in the initial release version of Exchange 2010:</span></span> <ul> <li>  <span data-ttu-id="10ac7-156">Liste de Distribution privée complète</span><span class="sxs-lookup"><span data-stu-id="10ac7-156">Full Private Distribution List</span></span></li><li><span data-ttu-id="10ac7-157">Objets de Configuration utilisateur</span><span class="sxs-lookup"><span data-stu-id="10ac7-157">User Configuration Objects</span></span></li><li><span data-ttu-id="10ac7-158">Dossier des éléments associés</span><span class="sxs-lookup"><span data-stu-id="10ac7-158">Folder Associated Items</span></span></li><li><span data-ttu-id="10ac7-159">Suivi des messages</span><span class="sxs-lookup"><span data-stu-id="10ac7-159">Message tracking</span></span></li><li><span data-ttu-id="10ac7-160">Messagerie unifiée</span><span class="sxs-lookup"><span data-stu-id="10ac7-160">Unified Messaging</span></span></li><li><span data-ttu-id="10ac7-161">Découverte automatique SOAP</span><span class="sxs-lookup"><span data-stu-id="10ac7-161">SOAP Autodiscover</span></span>  </li><li><span data-ttu-id="10ac7-162">Prise en charge améliorée de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="10ac7-162">Enhanced Time Zone support</span></span></li><li><span data-ttu-id="10ac7-163">Informations de disponibilité de ressources de salle</span><span class="sxs-lookup"><span data-stu-id="10ac7-163">Room resource availability information</span></span></li><li><span data-ttu-id="10ac7-164">Recherche indexés</span><span class="sxs-lookup"><span data-stu-id="10ac7-164">Indexed search</span></span></li><li><span data-ttu-id="10ac7-165">Accès benne</span><span class="sxs-lookup"><span data-stu-id="10ac7-165">Dumpster access</span></span></li><li><span data-ttu-id="10ac7-166">Partage des informations</span><span class="sxs-lookup"><span data-stu-id="10ac7-166">MailTips information</span></span></li></ul> |
|<span data-ttu-id="10ac7-167">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="10ac7-167">Exchange 2007 SP1</span></span>  | <span data-ttu-id="10ac7-168">Inclut toutes les fonctionnalités introduites dans Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="10ac7-168">Includes all the features introduced in Exchange 2007.</span></span> <span data-ttu-id="10ac7-169">Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-169">The following features were introduced in Exchange 2007 SP1:</span></span>  <ul><li>  <span data-ttu-id="10ac7-170">Gestion des délégués</span><span class="sxs-lookup"><span data-stu-id="10ac7-170">Delegate management</span></span></li><li><span data-ttu-id="10ac7-171">Autorisations de dossier</span><span class="sxs-lookup"><span data-stu-id="10ac7-171">Folder permissions</span></span></li><li><span data-ttu-id="10ac7-172">Dossiers publics</span><span class="sxs-lookup"><span data-stu-id="10ac7-172">Public folders</span></span></li><li><span data-ttu-id="10ac7-173">Publier des éléments</span><span class="sxs-lookup"><span data-stu-id="10ac7-173">Post items</span></span></li><li><span data-ttu-id="10ac7-174">Conversion de l’ID</span><span class="sxs-lookup"><span data-stu-id="10ac7-174">ID conversion</span></span></li></ul> |
|<span data-ttu-id="10ac7-175">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="10ac7-175">Exchange 2007</span></span>  | <span data-ttu-id="10ac7-176">Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2007 :</span><span class="sxs-lookup"><span data-stu-id="10ac7-176">The following features were introduced in the initial release version of Exchange 2007:</span></span>  <ul><li>  <span data-ttu-id="10ac7-177">Accès total aux éléments, dossiers et pièces jointes (créer, obtenir, mettre à jour, supprimer)</span><span class="sxs-lookup"><span data-stu-id="10ac7-177">Full access to items, folders, and attachments (Create, Get, Update, Delete)</span></span></li><li><span data-ttu-id="10ac7-178">Disponibilité</span><span class="sxs-lookup"><span data-stu-id="10ac7-178">Availability</span></span></li><li><span data-ttu-id="10ac7-179">En dehors des paramètres Office</span><span class="sxs-lookup"><span data-stu-id="10ac7-179">Out of Office settings</span></span></li><li><span data-ttu-id="10ac7-180">Notifications</span><span class="sxs-lookup"><span data-stu-id="10ac7-180">Notifications</span></span></li><li><span data-ttu-id="10ac7-181">Synchronisation</span><span class="sxs-lookup"><span data-stu-id="10ac7-181">Synchronization</span></span></li><li><span data-ttu-id="10ac7-182">Résolution de noms</span><span class="sxs-lookup"><span data-stu-id="10ac7-182">Name resolution</span></span></li><li><span data-ttu-id="10ac7-183">Extension de la distribution (liste)</span><span class="sxs-lookup"><span data-stu-id="10ac7-183">Distribution list (DL) expansion</span></span></li><li><span data-ttu-id="10ac7-184">Search</span><span class="sxs-lookup"><span data-stu-id="10ac7-184">Search</span></span></li></ul> |
   
## <a name="see-also"></a><span data-ttu-id="10ac7-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10ac7-185">See also</span></span>

- [<span data-ttu-id="10ac7-186">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="10ac7-186">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="10ac7-187">Migration et les technologies Exchange</span><span class="sxs-lookup"><span data-stu-id="10ac7-187">Migrating to Exchange technologies</span></span>](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [<span data-ttu-id="10ac7-188">Explorer l'API managée EWS, EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="10ac7-188">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    
