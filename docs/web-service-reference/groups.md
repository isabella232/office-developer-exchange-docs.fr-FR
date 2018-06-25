---
title: Groupes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: L’élément groupes contient une collection des groupes qui sont trouvés dans les critères de recherche et d’agrégation identifiée dans la requête d’opération FindItem.
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827786"
---
# <a name="groups"></a><span data-ttu-id="ebfea-103">Groupes</span><span class="sxs-lookup"><span data-stu-id="ebfea-103">Groups</span></span>

<span data-ttu-id="ebfea-104">L’élément **groupes** contient une collection des groupes qui sont trouvés dans les critères de recherche et d’agrégation identifiée dans la requête [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ebfea-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="ebfea-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="ebfea-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebfea-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebfea-106">Attributes and elements</span></span>

<span data-ttu-id="ebfea-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebfea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebfea-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebfea-108">Attributes</span></span>

<span data-ttu-id="ebfea-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebfea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebfea-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebfea-110">Child elements</span></span>

|<span data-ttu-id="ebfea-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebfea-111">**Element**</span></span>|<span data-ttu-id="ebfea-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebfea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebfea-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="ebfea-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="ebfea-114">Représente une collection d’éléments qui sont le résultat d’une [opération FindItem](finditem-operation.md) groupée appeler.</span><span class="sxs-lookup"><span data-stu-id="ebfea-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ebfea-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebfea-115">Parent elements</span></span>

|<span data-ttu-id="ebfea-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebfea-116">**Element**</span></span>|<span data-ttu-id="ebfea-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebfea-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebfea-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ebfea-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="ebfea-119">Contient les résultats de la recherche d’un dossier racine unique pendant une [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ebfea-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ebfea-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ebfea-120">Remarks</span></span>

<span data-ttu-id="ebfea-121">Une seule instance [GroupedItems](groupeditems.md) se produit pour chaque groupe distinct dans le résultat.</span><span class="sxs-lookup"><span data-stu-id="ebfea-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="ebfea-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ebfea-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebfea-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebfea-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebfea-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebfea-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebfea-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebfea-125">Schema name</span></span>  <br/> |<span data-ttu-id="ebfea-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ebfea-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebfea-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebfea-127">Validation file</span></span>  <br/> |<span data-ttu-id="ebfea-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ebfea-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ebfea-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebfea-129">Can be empty</span></span>  <br/> |<span data-ttu-id="ebfea-130">False</span><span class="sxs-lookup"><span data-stu-id="ebfea-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebfea-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ebfea-131">See also</span></span>



[<span data-ttu-id="ebfea-132">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="ebfea-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="ebfea-133">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="ebfea-133">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

