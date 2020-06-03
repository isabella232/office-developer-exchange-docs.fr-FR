---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: L’élément FractionalPageItemView décrit l’emplacement où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une demande FindItem.
ms.openlocfilehash: cbf45838558873dc5846823c2d1b26cf2c8af514
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461309"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="900ec-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="900ec-103">FractionalPageItemView</span></span>

<span data-ttu-id="900ec-104">L’élément **FractionalPageItemView** décrit l’emplacement où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une demande [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="900ec-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="900ec-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="900ec-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="900ec-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="900ec-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="900ec-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="900ec-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="900ec-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="900ec-108">Attributes and elements</span></span>

<span data-ttu-id="900ec-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="900ec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="900ec-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="900ec-110">Attributes</span></span>

|<span data-ttu-id="900ec-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="900ec-111">**Attribute**</span></span>|<span data-ttu-id="900ec-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="900ec-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="900ec-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="900ec-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="900ec-114">Identifie le nombre maximal de résultats à renvoyer dans la réponse [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="900ec-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="900ec-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="900ec-115">This attribute is optional.</span></span> <span data-ttu-id="900ec-116">Si cet attribut n’est pas spécifié, l’appel renverra tous les éléments disponibles.</span><span class="sxs-lookup"><span data-stu-id="900ec-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="900ec-117">**Monnaie**</span><span class="sxs-lookup"><span data-stu-id="900ec-117">**Numerator**</span></span> <br/> |<span data-ttu-id="900ec-118">Représente le numérateur du décalage fractionnaire à partir du début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="900ec-119">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="900ec-119">This attribute is required.</span></span> <span data-ttu-id="900ec-120">Le numérateur doit être inférieur ou égal au dénominateur.</span><span class="sxs-lookup"><span data-stu-id="900ec-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="900ec-121">Cet attribut doit représenter une valeur intégrale égale ou supérieure à zéro.</span><span class="sxs-lookup"><span data-stu-id="900ec-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="900ec-122">Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="900ec-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="900ec-123">**Petit**</span><span class="sxs-lookup"><span data-stu-id="900ec-123">**Denominator**</span></span> <br/> |<span data-ttu-id="900ec-124">Représente le dénominateur du décalage fractionnaire à partir du début du nombre total d’éléments dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="900ec-125">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="900ec-125">This attribute is required.</span></span> <span data-ttu-id="900ec-126">Cet attribut doit représenter une valeur intégrale supérieure à 1.</span><span class="sxs-lookup"><span data-stu-id="900ec-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="900ec-127">Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="900ec-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="900ec-128">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="900ec-128">Child elements</span></span>

<span data-ttu-id="900ec-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="900ec-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="900ec-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="900ec-130">Parent elements</span></span>

|<span data-ttu-id="900ec-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="900ec-131">**Element**</span></span>|<span data-ttu-id="900ec-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="900ec-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="900ec-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="900ec-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="900ec-134">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="900ec-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="900ec-135">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="900ec-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="900ec-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="900ec-136">Remarks</span></span>

<span data-ttu-id="900ec-137">Le décalage de l’affichage paginé à partir du début de l’ensemble des éléments trouvés est décrit par une fraction.</span><span class="sxs-lookup"><span data-stu-id="900ec-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="900ec-138">La fraction, définie par les attributs **numérateur** et **dénominateur** , décrit l’emplacement de début de la page d’informations.</span><span class="sxs-lookup"><span data-stu-id="900ec-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="900ec-139">Par exemple, si le **numérateur** est égal à quatre et que le **dénominateur** est égal à cinq, la page des informations retournées commence à une entrée située quatre cinquièmes du contenu du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="900ec-140">Si la fraction est égale à zéro, cela indique le début du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="900ec-141">Si la fraction est égale à 1, cela indique la fin du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="900ec-142">La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="900ec-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="900ec-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="900ec-144">Exemple</span><span class="sxs-lookup"><span data-stu-id="900ec-144">Example</span></span>

<span data-ttu-id="900ec-145">L’exemple suivant montre une requête [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="900ec-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="900ec-146">La requête renvoie les éléments à partir des résultats de la recherche qui commencent après le deuxième tiers de tous les éléments du jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
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
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
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

<span data-ttu-id="900ec-147">Par exemple, si le jeu de résultats contient neuf éléments, la vue paginée renverra jusqu’à 12 éléments, à partir de l’élément a trouvé deux-tiers de la méthode dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="900ec-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="900ec-148">Dans ce cas, la page commence au septième élément.</span><span class="sxs-lookup"><span data-stu-id="900ec-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="900ec-149">La page contiendra les septième, huitième et neuvième éléments.</span><span class="sxs-lookup"><span data-stu-id="900ec-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="900ec-150">Si le numérateur est défini sur zéro, l’affichage de la page renverra tous les éléments dans le jeu de résultats tant que le nombre est inférieur à l’attribut **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="900ec-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="900ec-151">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="900ec-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="900ec-152">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="900ec-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="900ec-153">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="900ec-153">Schema Name</span></span>  <br/> |<span data-ttu-id="900ec-154">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="900ec-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="900ec-155">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="900ec-155">Validation File</span></span>  <br/> |<span data-ttu-id="900ec-156">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="900ec-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="900ec-157">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="900ec-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="900ec-158">False</span><span class="sxs-lookup"><span data-stu-id="900ec-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="900ec-159">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="900ec-159">See also</span></span>



[<span data-ttu-id="900ec-160">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="900ec-160">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="900ec-161">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="900ec-161">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

