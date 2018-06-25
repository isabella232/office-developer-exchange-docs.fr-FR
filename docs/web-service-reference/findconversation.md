---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: L’élément FindConversation définit une requête pour rechercher les conversations dans une boîte aux lettres.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756381"
---
# <a name="findconversation"></a><span data-ttu-id="50c9e-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="50c9e-103">FindConversation</span></span>

<span data-ttu-id="50c9e-104">L’élément **FindConversation** définit une requête pour rechercher les conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="50c9e-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="50c9e-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="50c9e-105">FindConversation</span></span>](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 <span data-ttu-id="50c9e-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="50c9e-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50c9e-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50c9e-107">Attributes and elements</span></span>

<span data-ttu-id="50c9e-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50c9e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50c9e-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="50c9e-109">Attributes</span></span>

****

|<span data-ttu-id="50c9e-110">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="50c9e-110">**Attribute**</span></span>|<span data-ttu-id="50c9e-111">**Description**</span><span class="sxs-lookup"><span data-stu-id="50c9e-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50c9e-112">Traversée du contenu</span><span class="sxs-lookup"><span data-stu-id="50c9e-112">Traversal</span></span>  <br/> |<span data-ttu-id="50c9e-113">Identifie les types de parcours sous-arborescence.</span><span class="sxs-lookup"><span data-stu-id="50c9e-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="50c9e-114">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="50c9e-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="50c9e-115">AffichageFiltrer</span><span class="sxs-lookup"><span data-stu-id="50c9e-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="50c9e-116">Identifie les filtres d’affichage types.</span><span class="sxs-lookup"><span data-stu-id="50c9e-116">Identifies the types view filters.</span></span> <span data-ttu-id="50c9e-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="50c9e-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="50c9e-118">Valeurs d’attribut Traversal</span><span class="sxs-lookup"><span data-stu-id="50c9e-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="50c9e-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="50c9e-119">**Value**</span></span>|<span data-ttu-id="50c9e-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="50c9e-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50c9e-121">Peu profond</span><span class="sxs-lookup"><span data-stu-id="50c9e-121">Shallow</span></span>  <br/> |<span data-ttu-id="50c9e-122">Indique un parcours en surface.</span><span class="sxs-lookup"><span data-stu-id="50c9e-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="50c9e-123">Profond</span><span class="sxs-lookup"><span data-stu-id="50c9e-123">Deep</span></span>  <br/> |<span data-ttu-id="50c9e-124">Indique un parcours en profondeur.</span><span class="sxs-lookup"><span data-stu-id="50c9e-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="50c9e-125">Valeurs des attributs AffichageFiltrer</span><span class="sxs-lookup"><span data-stu-id="50c9e-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="50c9e-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="50c9e-126">**Value**</span></span>|<span data-ttu-id="50c9e-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="50c9e-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50c9e-128">Tous</span><span class="sxs-lookup"><span data-stu-id="50c9e-128">All</span></span>  <br/> |<span data-ttu-id="50c9e-129">Recherchez toutes les conversations.</span><span class="sxs-lookup"><span data-stu-id="50c9e-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="50c9e-130">Marqué d’un indicateur</span><span class="sxs-lookup"><span data-stu-id="50c9e-130">Flagged</span></span>  <br/> |<span data-ttu-id="50c9e-131">Rechercher les conversations avec indicateur.</span><span class="sxs-lookup"><span data-stu-id="50c9e-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="50c9e-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="50c9e-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="50c9e-133">Rechercher les conversations avec les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="50c9e-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="50c9e-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="50c9e-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="50c9e-135">Rechercher les conversations adressé ou cc serait Me.</span><span class="sxs-lookup"><span data-stu-id="50c9e-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="50c9e-136">Unread</span><span class="sxs-lookup"><span data-stu-id="50c9e-136">Unread</span></span>  <br/> |<span data-ttu-id="50c9e-137">Rechercher les conversations non lues.</span><span class="sxs-lookup"><span data-stu-id="50c9e-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="50c9e-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="50c9e-138">TaskActive</span></span>  <br/> |<span data-ttu-id="50c9e-139">Rechercher des tâches actives.</span><span class="sxs-lookup"><span data-stu-id="50c9e-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="50c9e-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="50c9e-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="50c9e-141">Rechercher les tâches en retard.</span><span class="sxs-lookup"><span data-stu-id="50c9e-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="50c9e-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="50c9e-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="50c9e-143">Rechercher les tâches terminées.</span><span class="sxs-lookup"><span data-stu-id="50c9e-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="50c9e-144">NoClutter</span><span class="sxs-lookup"><span data-stu-id="50c9e-144">NoClutter</span></span>  <br/> |<span data-ttu-id="50c9e-145">Réservé à un usage interne</span><span class="sxs-lookup"><span data-stu-id="50c9e-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="50c9e-146">Encombrement</span><span class="sxs-lookup"><span data-stu-id="50c9e-146">Clutter</span></span>  <br/> |<span data-ttu-id="50c9e-147">Réservé à un usage interne</span><span class="sxs-lookup"><span data-stu-id="50c9e-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="50c9e-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50c9e-148">Child elements</span></span>

|<span data-ttu-id="50c9e-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50c9e-149">**Element**</span></span>|<span data-ttu-id="50c9e-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="50c9e-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50c9e-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="50c9e-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="50c9e-152">Décrit comment paginée conversation les informations sont retournées.</span><span class="sxs-lookup"><span data-stu-id="50c9e-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="50c9e-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="50c9e-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="50c9e-154">Spécifie la condition qui sert à identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="50c9e-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="50c9e-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="50c9e-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="50c9e-156">Définit comment les éléments sont triés dans une requête [d’opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50c9e-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="50c9e-157">La propriété **conversation : LastDeliveryTime** est la seule propriété qui est pris en charge pour le tri lors de l’opération **FindConversation** est utilisée.</span><span class="sxs-lookup"><span data-stu-id="50c9e-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="50c9e-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="50c9e-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="50c9e-159">Identifie le dossier pour rechercher des conversations.</span><span class="sxs-lookup"><span data-stu-id="50c9e-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="50c9e-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="50c9e-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="50c9e-161">Spécifie si une recherche ou extraction d’une conversation doit couvrir la boîte aux lettres principale, boîte aux lettres d’archivage ou les deux principal et archiver des boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="50c9e-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="50c9e-162">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="50c9e-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="50c9e-163">Spécifie une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="50c9e-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="50c9e-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="50c9e-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="50c9e-165">Identifie la propriété définie pour retourner une réponse de [l’opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50c9e-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50c9e-166">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50c9e-166">Parent elements</span></span>

<span data-ttu-id="50c9e-167">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50c9e-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="50c9e-168">Remarques</span><span class="sxs-lookup"><span data-stu-id="50c9e-168">Remarks</span></span>

<span data-ttu-id="50c9e-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="50c9e-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50c9e-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50c9e-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50c9e-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50c9e-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50c9e-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50c9e-172">Schema Name</span></span>  <br/> |<span data-ttu-id="50c9e-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="50c9e-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50c9e-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50c9e-174">Validation File</span></span>  <br/> |<span data-ttu-id="50c9e-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="50c9e-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50c9e-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50c9e-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="50c9e-177">False</span><span class="sxs-lookup"><span data-stu-id="50c9e-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50c9e-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50c9e-178">See also</span></span>



[<span data-ttu-id="50c9e-179">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="50c9e-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="50c9e-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="50c9e-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="50c9e-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="50c9e-181">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

