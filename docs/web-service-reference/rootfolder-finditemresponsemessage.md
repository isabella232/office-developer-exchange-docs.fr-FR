---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique lors d’une opération FindItem.
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829254"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="65e98-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="65e98-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="65e98-104">L’élément **RootFolder** contient les résultats d’une recherche d’un dossier racine unique lors d’une [opération FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="65e98-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="65e98-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="65e98-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65e98-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65e98-106">Attributes and elements</span></span>

<span data-ttu-id="65e98-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65e98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65e98-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65e98-108">Attributes</span></span>

|<span data-ttu-id="65e98-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="65e98-109">**Attribute**</span></span>|<span data-ttu-id="65e98-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="65e98-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65e98-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="65e98-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="65e98-112">Représente l’index suivant doit être utilisé pour la requête suivante lors de l’utilisation d’une vue indexée de pagination.</span><span class="sxs-lookup"><span data-stu-id="65e98-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="65e98-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="65e98-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="65e98-114">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lors de l’utilisation des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="65e98-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="65e98-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="65e98-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="65e98-116">Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination en fraction.</span><span class="sxs-lookup"><span data-stu-id="65e98-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="65e98-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="65e98-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="65e98-118">Indique si les résultats actuels contient le dernier élément dans la requête, telles que davantage de pagination n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="65e98-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="65e98-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="65e98-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="65e98-120">Représente le nombre total d’éléments qui transmet la restriction.</span><span class="sxs-lookup"><span data-stu-id="65e98-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="65e98-121">Dans une [opération FindItem](finditem-operation.md)groupée, l’attribut **TotalItemsInView** renvoie le nombre total d’éléments dans la vue ainsi que le nombre total de groupes.</span><span class="sxs-lookup"><span data-stu-id="65e98-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="65e98-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65e98-122">Child elements</span></span>

|<span data-ttu-id="65e98-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65e98-123">**Element**</span></span>|<span data-ttu-id="65e98-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="65e98-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65e98-125">Items</span><span class="sxs-lookup"><span data-stu-id="65e98-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="65e98-126">Contient un tableau d’éléments trouvés dont les critères de recherche identifiés dans la requête [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65e98-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="65e98-127">Groupes</span><span class="sxs-lookup"><span data-stu-id="65e98-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="65e98-128">Contient une collection de groupes trouvés dont les critères de recherche et d’agrégation identifiés dans la requête [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65e98-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65e98-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65e98-129">Parent elements</span></span>

|<span data-ttu-id="65e98-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65e98-130">**Element**</span></span>|<span data-ttu-id="65e98-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="65e98-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65e98-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65e98-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="65e98-133">Contient l’état et les résultats d’une demande [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65e98-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65e98-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="65e98-134">Remarks</span></span>

<span data-ttu-id="65e98-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="65e98-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65e98-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65e98-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65e98-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65e98-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65e98-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65e98-138">Schema name</span></span>  <br/> |<span data-ttu-id="65e98-139">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="65e98-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="65e98-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65e98-140">Validation file</span></span>  <br/> |<span data-ttu-id="65e98-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="65e98-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65e98-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65e98-142">Can be empty</span></span>  <br/> |<span data-ttu-id="65e98-143">False</span><span class="sxs-lookup"><span data-stu-id="65e98-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65e98-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65e98-144">See also</span></span>



[<span data-ttu-id="65e98-145">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="65e98-145">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="65e98-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="65e98-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="65e98-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="65e98-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="65e98-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="65e98-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="65e98-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="65e98-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="65e98-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="65e98-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="65e98-151">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="65e98-151">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

