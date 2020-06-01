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
description: L’élément FindConversation définit une requête pour rechercher des conversations dans une boîte aux lettres.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462646"
---
# <a name="findconversation"></a><span data-ttu-id="a7edf-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="a7edf-103">FindConversation</span></span>

<span data-ttu-id="a7edf-104">L’élément **FindConversation** définit une requête pour rechercher des conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a7edf-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="a7edf-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="a7edf-105">FindConversation</span></span>](findconversation.md)
  
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

 <span data-ttu-id="a7edf-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="a7edf-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7edf-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7edf-107">Attributes and elements</span></span>

<span data-ttu-id="a7edf-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7edf-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7edf-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7edf-109">Attributes</span></span>

****

|<span data-ttu-id="a7edf-110">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a7edf-110">**Attribute**</span></span>|<span data-ttu-id="a7edf-111">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7edf-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7edf-112">Traversée</span><span class="sxs-lookup"><span data-stu-id="a7edf-112">Traversal</span></span>  <br/> |<span data-ttu-id="a7edf-113">Identifie les types de parcours de sous-arborescence.</span><span class="sxs-lookup"><span data-stu-id="a7edf-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="a7edf-114">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a7edf-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a7edf-115">ViewFilter</span><span class="sxs-lookup"><span data-stu-id="a7edf-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="a7edf-116">Identifie les filtres d’affichage de types.</span><span class="sxs-lookup"><span data-stu-id="a7edf-116">Identifies the types view filters.</span></span> <span data-ttu-id="a7edf-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a7edf-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="a7edf-118">Valeurs d’attribut transversal</span><span class="sxs-lookup"><span data-stu-id="a7edf-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="a7edf-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a7edf-119">**Value**</span></span>|<span data-ttu-id="a7edf-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7edf-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7edf-121">Partielle</span><span class="sxs-lookup"><span data-stu-id="a7edf-121">Shallow</span></span>  <br/> |<span data-ttu-id="a7edf-122">Indique un parcours superficiel.</span><span class="sxs-lookup"><span data-stu-id="a7edf-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="a7edf-123">Développée</span><span class="sxs-lookup"><span data-stu-id="a7edf-123">Deep</span></span>  <br/> |<span data-ttu-id="a7edf-124">Indique un parcours approfondi.</span><span class="sxs-lookup"><span data-stu-id="a7edf-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="a7edf-125">Valeurs d’attribut ViewFilter</span><span class="sxs-lookup"><span data-stu-id="a7edf-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="a7edf-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a7edf-126">**Value**</span></span>|<span data-ttu-id="a7edf-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7edf-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7edf-128">Tous</span><span class="sxs-lookup"><span data-stu-id="a7edf-128">All</span></span>  <br/> |<span data-ttu-id="a7edf-129">Rechercher toutes les conversations.</span><span class="sxs-lookup"><span data-stu-id="a7edf-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="a7edf-130">Marqué d’un indicateur</span><span class="sxs-lookup"><span data-stu-id="a7edf-130">Flagged</span></span>  <br/> |<span data-ttu-id="a7edf-131">Rechercher des conversations avec indicateur.</span><span class="sxs-lookup"><span data-stu-id="a7edf-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="a7edf-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="a7edf-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="a7edf-133">Rechercher des conversations avec des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="a7edf-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="a7edf-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="a7edf-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="a7edf-135">Rechercher les conversations adressées ou CC avec moi.</span><span class="sxs-lookup"><span data-stu-id="a7edf-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="a7edf-136">Non lus</span><span class="sxs-lookup"><span data-stu-id="a7edf-136">Unread</span></span>  <br/> |<span data-ttu-id="a7edf-137">Rechercher des conversations non lues.</span><span class="sxs-lookup"><span data-stu-id="a7edf-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="a7edf-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="a7edf-138">TaskActive</span></span>  <br/> |<span data-ttu-id="a7edf-139">Rechercher des tâches actives.</span><span class="sxs-lookup"><span data-stu-id="a7edf-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="a7edf-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="a7edf-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="a7edf-141">Recherchez les tâches en retard.</span><span class="sxs-lookup"><span data-stu-id="a7edf-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="a7edf-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="a7edf-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="a7edf-143">Recherchez les tâches terminées.</span><span class="sxs-lookup"><span data-stu-id="a7edf-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="a7edf-144">Nodésordre</span><span class="sxs-lookup"><span data-stu-id="a7edf-144">NoClutter</span></span>  <br/> |<span data-ttu-id="a7edf-145">À usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="a7edf-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="a7edf-146">Courrier non trié</span><span class="sxs-lookup"><span data-stu-id="a7edf-146">Clutter</span></span>  <br/> |<span data-ttu-id="a7edf-147">À usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="a7edf-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a7edf-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7edf-148">Child elements</span></span>

|<span data-ttu-id="a7edf-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7edf-149">**Element**</span></span>|<span data-ttu-id="a7edf-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7edf-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7edf-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="a7edf-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="a7edf-152">Indique comment les informations de conversation paginée sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="a7edf-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="a7edf-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="a7edf-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="a7edf-154">Spécifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et l’orientation de la recherche pour une recherche **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="a7edf-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="a7edf-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="a7edf-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="a7edf-156">Définit le mode de tri des éléments dans une demande d' [opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a7edf-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="a7edf-157">La propriété **conversation : LastDeliveryTime** est la seule propriété prise en charge pour le tri lorsque l’opération **FindConversation** est utilisée.</span><span class="sxs-lookup"><span data-stu-id="a7edf-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="a7edf-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="a7edf-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="a7edf-159">Identifie le dossier dans lequel Rechercher des conversations.</span><span class="sxs-lookup"><span data-stu-id="a7edf-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="a7edf-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="a7edf-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="a7edf-161">Indique si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux.</span><span class="sxs-lookup"><span data-stu-id="a7edf-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a7edf-162">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="a7edf-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="a7edf-163">Spécifie une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="a7edf-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="a7edf-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="a7edf-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="a7edf-165">Identifie le jeu de propriétés à renvoyer dans une réponse d' [opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a7edf-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7edf-166">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7edf-166">Parent elements</span></span>

<span data-ttu-id="a7edf-167">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7edf-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7edf-168">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7edf-168">Remarks</span></span>

<span data-ttu-id="a7edf-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a7edf-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7edf-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7edf-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7edf-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7edf-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a7edf-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7edf-172">Schema Name</span></span>  <br/> |<span data-ttu-id="a7edf-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a7edf-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a7edf-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7edf-174">Validation File</span></span>  <br/> |<span data-ttu-id="a7edf-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a7edf-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a7edf-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7edf-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7edf-177">False</span><span class="sxs-lookup"><span data-stu-id="a7edf-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7edf-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a7edf-178">See also</span></span>



[<span data-ttu-id="a7edf-179">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="a7edf-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="a7edf-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a7edf-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a7edf-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="a7edf-181">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

