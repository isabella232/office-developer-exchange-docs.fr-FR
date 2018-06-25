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
description: L’élément GroupedItems représente une collection d’éléments qui sont le résultat d’un appel d’opération FindItem groupé.
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827756"
---
# <a name="groupeditems"></a><span data-ttu-id="ef97c-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="ef97c-103">GroupedItems</span></span>

<span data-ttu-id="ef97c-104">L’élément **GroupedItems** représente une collection d’éléments qui sont le résultat d’une [opération FindItem](finditem-operation.md) groupée d’appel.</span><span class="sxs-lookup"><span data-stu-id="ef97c-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="ef97c-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="ef97c-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="ef97c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef97c-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="ef97c-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef97c-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="ef97c-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ef97c-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="ef97c-109">Groupes</span><span class="sxs-lookup"><span data-stu-id="ef97c-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="ef97c-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="ef97c-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="ef97c-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="ef97c-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef97c-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ef97c-112">Attributes and elements</span></span>

<span data-ttu-id="ef97c-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ef97c-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef97c-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="ef97c-114">Attributes</span></span>

<span data-ttu-id="ef97c-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ef97c-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef97c-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ef97c-116">Child elements</span></span>

|<span data-ttu-id="ef97c-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ef97c-117">**Element**</span></span>|<span data-ttu-id="ef97c-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ef97c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef97c-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="ef97c-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="ef97c-120">Représente la valeur de la propriété qui est utilisé pour regrouper les éléments dans une [opération FindItem](finditem-operation.md) groupée d’appel.</span><span class="sxs-lookup"><span data-stu-id="ef97c-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="ef97c-121">Items</span><span class="sxs-lookup"><span data-stu-id="ef97c-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="ef97c-122">Contient un tableau d’éléments regroupés.</span><span class="sxs-lookup"><span data-stu-id="ef97c-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef97c-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ef97c-123">Parent elements</span></span>

|<span data-ttu-id="ef97c-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ef97c-124">**Element**</span></span>|<span data-ttu-id="ef97c-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="ef97c-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef97c-126">Groupes</span><span class="sxs-lookup"><span data-stu-id="ef97c-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="ef97c-127">Contient une collection des groupes qui sont trouvés dans les critères de recherche et d’agrégation identifiée dans la requête [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ef97c-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef97c-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="ef97c-128">Remarks</span></span>

<span data-ttu-id="ef97c-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ef97c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef97c-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ef97c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef97c-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ef97c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef97c-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ef97c-132">Schema name</span></span>  <br/> |<span data-ttu-id="ef97c-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ef97c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef97c-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ef97c-134">Validation file</span></span>  <br/> |<span data-ttu-id="ef97c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef97c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef97c-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ef97c-136">Can be empty</span></span>  <br/> |<span data-ttu-id="ef97c-137">False</span><span class="sxs-lookup"><span data-stu-id="ef97c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef97c-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ef97c-138">See also</span></span>



[<span data-ttu-id="ef97c-139">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="ef97c-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="ef97c-140">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="ef97c-140">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

