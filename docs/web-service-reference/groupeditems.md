---
title: GroupedItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: L’élément GroupedItems représente une collection d’éléments qui sont le résultat d’un appel d’opération groupée FindItem.
ms.openlocfilehash: 0ee1ca3c6d0cf98e2daefa60a1cb1fd096cda478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530810"
---
# <a name="groupeditems"></a><span data-ttu-id="9d713-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="9d713-103">GroupedItems</span></span>

<span data-ttu-id="9d713-104">L’élément **GroupedItems** représente une collection d’éléments qui sont le résultat d’un appel d' [opération](finditem-operation.md) groupée FindItem.</span><span class="sxs-lookup"><span data-stu-id="9d713-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="9d713-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="9d713-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="9d713-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9d713-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="9d713-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9d713-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="9d713-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="9d713-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="9d713-109">Groups</span><span class="sxs-lookup"><span data-stu-id="9d713-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="9d713-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="9d713-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="9d713-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="9d713-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d713-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9d713-112">Attributes and elements</span></span>

<span data-ttu-id="9d713-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9d713-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d713-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="9d713-114">Attributes</span></span>

<span data-ttu-id="9d713-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9d713-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d713-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9d713-116">Child elements</span></span>

|<span data-ttu-id="9d713-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d713-117">**Element**</span></span>|<span data-ttu-id="9d713-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d713-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d713-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="9d713-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="9d713-120">Représente la valeur de la propriété qui est utilisée pour regrouper des éléments dans un appel d' [opération FindItem](finditem-operation.md) groupé.</span><span class="sxs-lookup"><span data-stu-id="9d713-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="9d713-121">Items</span><span class="sxs-lookup"><span data-stu-id="9d713-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="9d713-122">Contient un tableau d’éléments groupés.</span><span class="sxs-lookup"><span data-stu-id="9d713-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d713-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9d713-123">Parent elements</span></span>

|<span data-ttu-id="9d713-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9d713-124">**Element**</span></span>|<span data-ttu-id="9d713-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="9d713-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d713-126">Groups</span><span class="sxs-lookup"><span data-stu-id="9d713-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="9d713-127">Contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9d713-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d713-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9d713-128">Remarks</span></span>

<span data-ttu-id="9d713-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9d713-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d713-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9d713-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d713-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9d713-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d713-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9d713-132">Schema name</span></span>  <br/> |<span data-ttu-id="9d713-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9d713-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d713-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9d713-134">Validation file</span></span>  <br/> |<span data-ttu-id="9d713-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d713-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d713-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9d713-136">Can be empty</span></span>  <br/> |<span data-ttu-id="9d713-137">False</span><span class="sxs-lookup"><span data-stu-id="9d713-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d713-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9d713-138">See also</span></span>



[<span data-ttu-id="9d713-139">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="9d713-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="9d713-140">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="9d713-140">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

