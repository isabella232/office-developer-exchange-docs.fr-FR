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
description: L’élément IndexedPageItemView décrit comment la conversation paginée ou les informations d’élément sont renvoyées pour une opération FindItem ou une demande d’opération FindConversation.
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456912"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="e436f-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="e436f-103">IndexedPageItemView</span></span>

<span data-ttu-id="e436f-104">L’élément **IndexedPageItemView** décrit comment la conversation paginée ou les informations d’élément sont renvoyées pour une [opération FindItem](finditem-operation.md) ou une demande d' [opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e436f-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="e436f-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="e436f-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e436f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e436f-106">Attributes and elements</span></span>

<span data-ttu-id="e436f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e436f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e436f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e436f-108">Attributes</span></span>

|<span data-ttu-id="e436f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e436f-109">**Attribute**</span></span>|<span data-ttu-id="e436f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e436f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e436f-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="e436f-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="e436f-112">Décrit le nombre maximal d’éléments ou de conversations à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="e436f-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="e436f-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e436f-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e436f-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="e436f-114">**Offset**</span></span> <br/> |<span data-ttu-id="e436f-115">Décrit le décalage par rapport à l' **BasePoint**.</span><span class="sxs-lookup"><span data-stu-id="e436f-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="e436f-116">Si **BasePoint** est égal à début, le décalage est positif.</span><span class="sxs-lookup"><span data-stu-id="e436f-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="e436f-117">Si **BasePoint** est égal à fin, le décalage est géré comme s’il était négatif.</span><span class="sxs-lookup"><span data-stu-id="e436f-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="e436f-118">Cela identifie l’élément ou la conversation qui sera le premier à être remis dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="e436f-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="e436f-119">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="e436f-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e436f-120">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="e436f-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="e436f-121">Indique si la page d’éléments ou de conversations commence à partir du début ou de la fin de l’ensemble d’éléments ou de conversations trouvé à l’aide des critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="e436f-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="e436f-122">La recherche à partir de la fin effectue toujours des recherches vers l’arrière.</span><span class="sxs-lookup"><span data-stu-id="e436f-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="e436f-123">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="e436f-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="e436f-124">Attribut BasePoint</span><span class="sxs-lookup"><span data-stu-id="e436f-124">BasePoint Attribute</span></span>

|<span data-ttu-id="e436f-125">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e436f-125">**Value**</span></span>|<span data-ttu-id="e436f-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="e436f-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e436f-127">Entam</span><span class="sxs-lookup"><span data-stu-id="e436f-127">Beginning</span></span>  <br/> |<span data-ttu-id="e436f-128">L’affichage paginé commence au début de la conversation ou de l’ensemble d’éléments trouvé.</span><span class="sxs-lookup"><span data-stu-id="e436f-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="e436f-129">End</span><span class="sxs-lookup"><span data-stu-id="e436f-129">End</span></span>  <br/> |<span data-ttu-id="e436f-130">L’affichage paginé commence à la fin de la conversation ou de l’ensemble d’éléments trouvé.</span><span class="sxs-lookup"><span data-stu-id="e436f-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e436f-131">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e436f-131">Child elements</span></span>

<span data-ttu-id="e436f-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e436f-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e436f-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e436f-133">Parent elements</span></span>

|<span data-ttu-id="e436f-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e436f-134">**Element**</span></span>|<span data-ttu-id="e436f-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="e436f-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e436f-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="e436f-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="e436f-137">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e436f-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="e436f-138">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e436f-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="e436f-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="e436f-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="e436f-140">Définit une requête pour rechercher des conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e436f-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e436f-141">Remarques</span><span class="sxs-lookup"><span data-stu-id="e436f-141">Remarks</span></span>

<span data-ttu-id="e436f-142">La recherche à partir de la fin implique le déplacement vers l’origine identifiée par le décalage.</span><span class="sxs-lookup"><span data-stu-id="e436f-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="e436f-143">De plus, le pointeur est ramené par le nombre d’enregistrements demandés.</span><span class="sxs-lookup"><span data-stu-id="e436f-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="e436f-144">Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 à partir de la fin, la recherche commence à partir de 75.</span><span class="sxs-lookup"><span data-stu-id="e436f-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="e436f-145">Si 10 enregistrements sont renvoyés, le pointeur de la souris recule de 10 enregistrements supplémentaires sur 65 et renvoie les enregistrements 65 à 75.</span><span class="sxs-lookup"><span data-stu-id="e436f-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="e436f-146">L’index suivant est 64.</span><span class="sxs-lookup"><span data-stu-id="e436f-146">The next index is 64.</span></span> <span data-ttu-id="e436f-147">Le prochain décalage par rapport à la fin d’une page est de 100 moins 64, ce qui équivaut à 36.</span><span class="sxs-lookup"><span data-stu-id="e436f-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="e436f-148">36 est la valeur du décalage suivant à partir de la fin pour obtenir la page indexée suivante.</span><span class="sxs-lookup"><span data-stu-id="e436f-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="e436f-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e436f-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="e436f-150">Exemple</span><span class="sxs-lookup"><span data-stu-id="e436f-150">Example</span></span>

<span data-ttu-id="e436f-151">L’exemple suivant montre une demande d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e436f-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="e436f-152">Chaque élément est renvoyé avec son ID et son objet.</span><span class="sxs-lookup"><span data-stu-id="e436f-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="e436f-153">Un maximum de six éléments sont renvoyés dans la réponse, comme spécifié par l’attribut **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="e436f-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="e436f-154">Les éléments sont répertoriés par ordre croissant groupés par importance.</span><span class="sxs-lookup"><span data-stu-id="e436f-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="e436f-155">Les éléments d’un groupe sont regroupés par objet.</span><span class="sxs-lookup"><span data-stu-id="e436f-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="e436f-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e436f-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e436f-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e436f-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e436f-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e436f-158">Schema Name</span></span>  <br/> |<span data-ttu-id="e436f-159">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e436f-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e436f-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e436f-160">Validation File</span></span>  <br/> |<span data-ttu-id="e436f-161">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e436f-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e436f-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e436f-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="e436f-163">False</span><span class="sxs-lookup"><span data-stu-id="e436f-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e436f-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e436f-164">See also</span></span>



[<span data-ttu-id="e436f-165">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="e436f-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="e436f-166">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="e436f-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="e436f-167">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="e436f-167">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

