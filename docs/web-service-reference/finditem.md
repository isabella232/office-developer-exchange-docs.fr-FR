---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: L’élément FindItem définit une demande pour rechercher des éléments dans une boîte aux lettres.
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460994"
---
# <a name="finditem"></a><span data-ttu-id="63abf-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="63abf-103">FindItem</span></span>

<span data-ttu-id="63abf-104">L’élément **FindItem** définit une demande pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="63abf-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


<span data-ttu-id="63abf-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="63abf-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63abf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63abf-106">Attributes and elements</span></span>

<span data-ttu-id="63abf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63abf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63abf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="63abf-108">Attributes</span></span>

|<span data-ttu-id="63abf-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="63abf-109">**Attribute**</span></span>|<span data-ttu-id="63abf-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="63abf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63abf-111">**Traversée**</span><span class="sxs-lookup"><span data-stu-id="63abf-111">**Traversal**</span></span> <br/> |<span data-ttu-id="63abf-112">Détermine si la recherche trouve des éléments dans des dossiers ou dans les bennes de dossiers.</span><span class="sxs-lookup"><span data-stu-id="63abf-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="63abf-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="63abf-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="63abf-114">Valeurs d’attribut transversal</span><span class="sxs-lookup"><span data-stu-id="63abf-114">Traversal attribute values</span></span>

|<span data-ttu-id="63abf-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="63abf-115">**Value**</span></span>|<span data-ttu-id="63abf-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="63abf-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63abf-117">Partielle</span><span class="sxs-lookup"><span data-stu-id="63abf-117">Shallow</span></span>  <br/> |<span data-ttu-id="63abf-118">Renvoie uniquement les identités des éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="63abf-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="63abf-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="63abf-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="63abf-120">Renvoie uniquement les identités des éléments situés dans la benne d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="63abf-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="63abf-121">Notez qu’une traversée supprimée de manière récupérable combinée à une restriction de recherche entraîne zéro élément retourné même s’il existe des éléments qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="63abf-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="63abf-122">Associé à</span><span class="sxs-lookup"><span data-stu-id="63abf-122">Associated</span></span>  <br/> |<span data-ttu-id="63abf-123">Renvoie uniquement les identités des éléments associés dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="63abf-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="63abf-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63abf-124">Child elements</span></span>

|<span data-ttu-id="63abf-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63abf-125">**Element**</span></span>|<span data-ttu-id="63abf-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="63abf-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63abf-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="63abf-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="63abf-128">Identifie les propriétés d’élément et le contenu à inclure dans une réponse d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="63abf-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="63abf-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="63abf-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="63abf-130">Décrit comment les informations d’élément paginé sont renvoyées pour une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="63abf-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="63abf-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="63abf-133">Décrit l’emplacement où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="63abf-134">Le décalage de l’affichage paginé à partir du début de l’ensemble des éléments trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="63abf-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="63abf-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="63abf-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="63abf-137">Fournit des limites de durée de temps pour définir une recherche pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="63abf-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="63abf-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="63abf-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="63abf-140">Définit une recherche pour les éléments de contact en fonction des noms d’affichage alphabétiques.</span><span class="sxs-lookup"><span data-stu-id="63abf-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="63abf-141">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="63abf-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="63abf-143">Spécifie des groupes arbitraires pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="63abf-144">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="63abf-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="63abf-146">Fournit des regroupements standard pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="63abf-147">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="63abf-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="63abf-149">Définit la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers **FindItem**dans /  les opérations FindItem**FindFolder** et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="63abf-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="63abf-150">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="63abf-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="63abf-152">Définit le mode de tri des éléments dans une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="63abf-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="63abf-153">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="63abf-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63abf-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="63abf-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="63abf-155">Identifie les dossiers dans lesquels rechercher les opérations FindItem et FindFolder.</span><span class="sxs-lookup"><span data-stu-id="63abf-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="63abf-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="63abf-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="63abf-157">Contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="63abf-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63abf-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63abf-158">Parent elements</span></span>

<span data-ttu-id="63abf-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63abf-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63abf-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="63abf-160">Remarks</span></span>

<span data-ttu-id="63abf-161">Un seul des éléments [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) peut être inclus dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="63abf-162">Un seul des éléments [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) peut être inclus dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="63abf-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="63abf-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="63abf-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63abf-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63abf-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63abf-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63abf-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63abf-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63abf-166">Schema Name</span></span>  <br/> |<span data-ttu-id="63abf-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="63abf-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63abf-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63abf-168">Validation File</span></span>  <br/> |<span data-ttu-id="63abf-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63abf-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63abf-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63abf-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="63abf-171">False</span><span class="sxs-lookup"><span data-stu-id="63abf-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63abf-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63abf-172">See also</span></span>

- [<span data-ttu-id="63abf-173">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="63abf-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="63abf-174">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="63abf-174">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

