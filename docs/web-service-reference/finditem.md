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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460994"
---
# <a name="finditem"></a><span data-ttu-id="36c3e-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="36c3e-103">FindItem</span></span>

<span data-ttu-id="36c3e-104">L’élément **FindItem** définit une demande pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="36c3e-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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


<span data-ttu-id="36c3e-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="36c3e-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36c3e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36c3e-106">Attributes and elements</span></span>

<span data-ttu-id="36c3e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36c3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36c3e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36c3e-108">Attributes</span></span>

|<span data-ttu-id="36c3e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="36c3e-109">**Attribute**</span></span>|<span data-ttu-id="36c3e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="36c3e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36c3e-111">**Traversée**</span><span class="sxs-lookup"><span data-stu-id="36c3e-111">**Traversal**</span></span> <br/> |<span data-ttu-id="36c3e-112">Détermine si la recherche trouve des éléments dans des dossiers ou dans les bennes de dossiers.</span><span class="sxs-lookup"><span data-stu-id="36c3e-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="36c3e-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="36c3e-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="36c3e-114">Valeurs d’attribut transversal</span><span class="sxs-lookup"><span data-stu-id="36c3e-114">Traversal attribute values</span></span>

|<span data-ttu-id="36c3e-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="36c3e-115">**Value**</span></span>|<span data-ttu-id="36c3e-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="36c3e-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36c3e-117">Partielle</span><span class="sxs-lookup"><span data-stu-id="36c3e-117">Shallow</span></span>  <br/> |<span data-ttu-id="36c3e-118">Renvoie uniquement les identités des éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="36c3e-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="36c3e-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="36c3e-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="36c3e-120">Renvoie uniquement les identités des éléments situés dans la benne d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="36c3e-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="36c3e-121">Notez qu’une traversée supprimée de manière récupérable combinée à une restriction de recherche entraîne zéro élément retourné même s’il existe des éléments qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="36c3e-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="36c3e-122">Associé à</span><span class="sxs-lookup"><span data-stu-id="36c3e-122">Associated</span></span>  <br/> |<span data-ttu-id="36c3e-123">Renvoie uniquement les identités des éléments associés dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="36c3e-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="36c3e-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36c3e-124">Child elements</span></span>

|<span data-ttu-id="36c3e-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36c3e-125">**Element**</span></span>|<span data-ttu-id="36c3e-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="36c3e-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36c3e-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="36c3e-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="36c3e-128">Identifie les propriétés d’élément et le contenu à inclure dans une réponse d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="36c3e-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="36c3e-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="36c3e-130">Décrit comment les informations d’élément paginé sont renvoyées pour une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="36c3e-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="36c3e-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="36c3e-133">Décrit l’emplacement où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="36c3e-134">Le décalage de l’affichage paginé à partir du début de l’ensemble des éléments trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="36c3e-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="36c3e-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="36c3e-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="36c3e-137">Fournit des limites de durée de temps pour définir une recherche pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="36c3e-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="36c3e-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="36c3e-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="36c3e-140">Définit une recherche pour les éléments de contact en fonction des noms d’affichage alphabétiques.</span><span class="sxs-lookup"><span data-stu-id="36c3e-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="36c3e-141">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="36c3e-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="36c3e-143">Spécifie des groupes arbitraires pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="36c3e-144">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="36c3e-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="36c3e-146">Fournit des regroupements standard pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="36c3e-147">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="36c3e-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="36c3e-149">Définit la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers **FindItem**dans /  les opérations FindItem**FindFolder** et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="36c3e-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="36c3e-150">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="36c3e-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="36c3e-152">Définit le mode de tri des éléments dans une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="36c3e-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="36c3e-153">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="36c3e-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="36c3e-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="36c3e-155">Identifie les dossiers dans lesquels rechercher les opérations FindItem et FindFolder.</span><span class="sxs-lookup"><span data-stu-id="36c3e-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="36c3e-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="36c3e-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="36c3e-157">Contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="36c3e-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36c3e-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36c3e-158">Parent elements</span></span>

<span data-ttu-id="36c3e-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36c3e-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36c3e-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="36c3e-160">Remarks</span></span>

<span data-ttu-id="36c3e-161">Un seul des éléments [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) peut être inclus dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="36c3e-162">Un seul des éléments [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) peut être inclus dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="36c3e-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="36c3e-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36c3e-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36c3e-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36c3e-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36c3e-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36c3e-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36c3e-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36c3e-166">Schema Name</span></span>  <br/> |<span data-ttu-id="36c3e-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="36c3e-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36c3e-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="36c3e-168">Validation File</span></span>  <br/> |<span data-ttu-id="36c3e-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="36c3e-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36c3e-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36c3e-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="36c3e-171">False</span><span class="sxs-lookup"><span data-stu-id="36c3e-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36c3e-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36c3e-172">See also</span></span>

- [<span data-ttu-id="36c3e-173">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="36c3e-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="36c3e-174">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="36c3e-174">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

