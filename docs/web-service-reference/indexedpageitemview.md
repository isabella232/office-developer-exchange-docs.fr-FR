---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: L’élément IndexedPageItemView décrit comment paginée conversation ou élément les informations sont retournées pour une opération FindItem ou une requête d’opération FindConversation.
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827919"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="4bcaa-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="4bcaa-103">IndexedPageItemView</span></span>

<span data-ttu-id="4bcaa-104">L’élément **IndexedPageItemView** décrit comment paginée conversation ou élément les informations sont retournées pour une demande [d’opération FindItem](finditem-operation.md) ou [FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4bcaa-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="4bcaa-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bcaa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4bcaa-106">Attributes and elements</span></span>

<span data-ttu-id="4bcaa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bcaa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4bcaa-108">Attributes</span></span>

|<span data-ttu-id="4bcaa-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-109">**Attribute**</span></span>|<span data-ttu-id="4bcaa-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4bcaa-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="4bcaa-112">Indique le nombre maximal d’éléments ou des conversations à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="4bcaa-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="4bcaa-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-114">**Offset**</span></span> <br/> |<span data-ttu-id="4bcaa-115">Indique le décalage à partir du **point de base**.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="4bcaa-116">Si le **point de base** est égal au début, le décalage est positif.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="4bcaa-117">Si le **point de base** est égal à End, le décalage est géré comme s’il s’agissait négatif.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="4bcaa-118">Il identifie l’élément ou conversation sera le premier à être remis dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="4bcaa-119">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4bcaa-120">**Point de base**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="4bcaa-121">Indique si la page des éléments ou des conversations redémarre depuis le début ou la fin de l’ensemble des éléments ou des conversations qui sont trouvent à l’aide de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="4bcaa-122">Recherche toujours à partir de la fin de recherche vers l’arrière.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="4bcaa-123">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="4bcaa-124">Attribut de point de base</span><span class="sxs-lookup"><span data-stu-id="4bcaa-124">BasePoint Attribute</span></span>

|<span data-ttu-id="4bcaa-125">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-125">**Value**</span></span>|<span data-ttu-id="4bcaa-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4bcaa-127">Début</span><span class="sxs-lookup"><span data-stu-id="4bcaa-127">Beginning</span></span>  <br/> |<span data-ttu-id="4bcaa-128">L’affichage paginé commence au début de l’ensemble de conversation ou d’un élément trouvé.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="4bcaa-129">End</span><span class="sxs-lookup"><span data-stu-id="4bcaa-129">End</span></span>  <br/> |<span data-ttu-id="4bcaa-130">L’affichage paginé commence à la fin de l’ensemble de conversation ou d’un élément trouvé.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4bcaa-131">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4bcaa-131">Child elements</span></span>

<span data-ttu-id="4bcaa-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4bcaa-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4bcaa-133">Parent elements</span></span>

|<span data-ttu-id="4bcaa-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-134">**Element**</span></span>|<span data-ttu-id="4bcaa-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="4bcaa-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bcaa-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="4bcaa-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="4bcaa-137">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="4bcaa-138">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="4bcaa-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="4bcaa-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="4bcaa-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="4bcaa-140">Définit une requête pour rechercher les conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bcaa-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="4bcaa-141">Remarks</span></span>

<span data-ttu-id="4bcaa-142">Recherche à partir de la fin consiste à déplacer à l’origine identifié par le décalage.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="4bcaa-143">En outre, le pointeur est ramené par le nombre d’enregistrements demandés.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="4bcaa-144">Par exemple, si 100 enregistrements et le décalage est de 25 à partir de la fin, la recherche démarre 75.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="4bcaa-145">Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière 10 supplémentaires à 65 des enregistrements et retourne les enregistrements de 65 à 75.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="4bcaa-146">L’index suivant est de 64.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-146">The next index is 64.</span></span> <span data-ttu-id="4bcaa-147">Le prochain offset à partir de la fin d’une page est de 100 moins 64 qui est égale à 36.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="4bcaa-148">36 est la valeur de décalage suivant à partir de la fin pour récupérer la page suivante indexée.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="4bcaa-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="4bcaa-150">Exemple</span><span class="sxs-lookup"><span data-stu-id="4bcaa-150">Example</span></span>

<span data-ttu-id="4bcaa-151">L’exemple suivant montre une demande [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4bcaa-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="4bcaa-152">Chaque élément est renvoyée avec son ID et son objet.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="4bcaa-153">Un maximum de six articles sont retournés dans la réponse, comme spécifié par l’attribut **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="4bcaa-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="4bcaa-154">Les éléments sont répertoriés dans l’ordre regroupé par importance croissant.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="4bcaa-155">Éléments d’un groupe sont regroupées par sujet.</span><span class="sxs-lookup"><span data-stu-id="4bcaa-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="4bcaa-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4bcaa-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bcaa-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4bcaa-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4bcaa-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4bcaa-158">Schema Name</span></span>  <br/> |<span data-ttu-id="4bcaa-159">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4bcaa-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4bcaa-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4bcaa-160">Validation File</span></span>  <br/> |<span data-ttu-id="4bcaa-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4bcaa-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4bcaa-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4bcaa-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="4bcaa-163">False</span><span class="sxs-lookup"><span data-stu-id="4bcaa-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4bcaa-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4bcaa-164">See also</span></span>



[<span data-ttu-id="4bcaa-165">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="4bcaa-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="4bcaa-166">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="4bcaa-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="4bcaa-167">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="4bcaa-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

