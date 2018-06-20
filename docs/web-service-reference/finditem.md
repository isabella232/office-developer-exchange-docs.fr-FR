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
description: L’élément FindItem définit une requête pour rechercher des éléments dans une boîte aux lettres.
ms.openlocfilehash: 9831b034be7deb0cf6e756bb585bdbe34b370afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756403"
---
# <a name="finditem"></a><span data-ttu-id="f4af4-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="f4af4-103">FindItem</span></span>

<span data-ttu-id="f4af4-104">L’élément **FindItem** définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f4af4-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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

 <span data-ttu-id="f4af4-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="f4af4-105">**FindItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4af4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f4af4-106">Attributes and elements</span></span>

<span data-ttu-id="f4af4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f4af4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4af4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f4af4-108">Attributes</span></span>

|<span data-ttu-id="f4af4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f4af4-109">**Attribute**</span></span>|<span data-ttu-id="f4af4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f4af4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4af4-111">**Traversée du contenu**</span><span class="sxs-lookup"><span data-stu-id="f4af4-111">**Traversal**</span></span> <br/> |<span data-ttu-id="f4af4-112">Définit si la recherche trouve des éléments dans les dossiers ou dumpsters des dossiers.</span><span class="sxs-lookup"><span data-stu-id="f4af4-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="f4af4-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="f4af4-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="f4af4-114">Valeurs d’attribut Traversal</span><span class="sxs-lookup"><span data-stu-id="f4af4-114">Traversal attribute values</span></span>

|<span data-ttu-id="f4af4-115">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f4af4-115">**Value**</span></span>|<span data-ttu-id="f4af4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="f4af4-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4af4-117">Peu profond</span><span class="sxs-lookup"><span data-stu-id="f4af4-117">Shallow</span></span>  <br/> |<span data-ttu-id="f4af4-118">Renvoie uniquement les identités des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="f4af4-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="f4af4-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="f4af4-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="f4af4-120">Renvoie uniquement les identités des éléments qui se trouvent dans un dossier de benne.</span><span class="sxs-lookup"><span data-stu-id="f4af4-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="f4af4-121">Notez que zéro renvoyés entraînera un parcours récupérable combiné à une restriction de recherche même s’il existe des éléments qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="f4af4-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="f4af4-122">Associé</span><span class="sxs-lookup"><span data-stu-id="f4af4-122">Associated</span></span>  <br/> |<span data-ttu-id="f4af4-123">Renvoie uniquement les identités des éléments associés dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="f4af4-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f4af4-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f4af4-124">Child elements</span></span>

|<span data-ttu-id="f4af4-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f4af4-125">**Element**</span></span>|<span data-ttu-id="f4af4-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="f4af4-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4af4-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="f4af4-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="f4af4-128">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse de [l’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f4af4-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="f4af4-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="f4af4-130">Décrit comment paginé informations sont retournées pour une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="f4af4-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="f4af4-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="f4af4-133">Décrit où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="f4af4-134">Le décalage d’affichage paginé depuis le début de l’ensemble des éléments trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="f4af4-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="f4af4-135">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="f4af4-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="f4af4-137">Fournit des temps couvrent des limites pour définir une recherche des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f4af4-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="f4af4-138">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="f4af4-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="f4af4-140">Définit une recherche des éléments de contact basées sur des noms d’affichage alphabétiques.</span><span class="sxs-lookup"><span data-stu-id="f4af4-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="f4af4-141">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="f4af4-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="f4af4-143">Spécifie les regroupements arbitraires pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="f4af4-144">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="f4af4-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="f4af4-146">Fournit des regroupements standards pour les requêtes **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="f4af4-147">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="f4af4-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f4af4-149">Définit la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans **FindItem**/ opérations de dossier**FindFolder** et la recherche.</span><span class="sxs-lookup"><span data-stu-id="f4af4-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="f4af4-150">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="f4af4-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="f4af4-152">Définit comment les éléments sont triés dans une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="f4af4-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="f4af4-153">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f4af4-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="f4af4-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="f4af4-155">Identifie les dossiers pour rechercher les opérations FindItem et FindFolder.</span><span class="sxs-lookup"><span data-stu-id="f4af4-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="f4af4-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="f4af4-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="f4af4-157">Contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="f4af4-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4af4-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f4af4-158">Parent elements</span></span>

<span data-ttu-id="f4af4-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f4af4-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4af4-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="f4af4-160">Remarks</span></span>

<span data-ttu-id="f4af4-161">Seul le [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou éléments [ContactsView](contactsview.md) peut être inclus dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="f4af4-162">Une seule des éléments [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) peut être incluse dans une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="f4af4-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="f4af4-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4af4-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4af4-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f4af4-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4af4-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f4af4-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4af4-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f4af4-166">Schema Name</span></span>  <br/> |<span data-ttu-id="f4af4-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f4af4-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4af4-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f4af4-168">Validation File</span></span>  <br/> |<span data-ttu-id="f4af4-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4af4-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4af4-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f4af4-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4af4-171">False</span><span class="sxs-lookup"><span data-stu-id="f4af4-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4af4-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f4af4-172">See also</span></span>



[<span data-ttu-id="f4af4-173">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="f4af4-173">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="f4af4-174">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="f4af4-174">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

