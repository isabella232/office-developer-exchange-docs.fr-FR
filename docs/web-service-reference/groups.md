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
description: L’élément Groups contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d’opération FindItem.
ms.openlocfilehash: 915d9dffd6d8cec1def6634e6b70642d563b5242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530788"
---
# <a name="groups"></a><span data-ttu-id="eafd8-103">Groupes</span><span class="sxs-lookup"><span data-stu-id="eafd8-103">Groups</span></span>

<span data-ttu-id="eafd8-104">L’élément **groups** contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="eafd8-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="eafd8-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="eafd8-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eafd8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eafd8-106">Attributes and elements</span></span>

<span data-ttu-id="eafd8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eafd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eafd8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="eafd8-108">Attributes</span></span>

<span data-ttu-id="eafd8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eafd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eafd8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eafd8-110">Child elements</span></span>

|<span data-ttu-id="eafd8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eafd8-111">**Element**</span></span>|<span data-ttu-id="eafd8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="eafd8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eafd8-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="eafd8-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="eafd8-114">Représente une collection d’éléments qui sont le résultat d’un appel d' [opération FindItem](finditem-operation.md) groupé.</span><span class="sxs-lookup"><span data-stu-id="eafd8-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eafd8-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eafd8-115">Parent elements</span></span>

|<span data-ttu-id="eafd8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eafd8-116">**Element**</span></span>|<span data-ttu-id="eafd8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="eafd8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eafd8-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="eafd8-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="eafd8-119">Contient les résultats d’une recherche d’un dossier racine unique pendant une opération d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="eafd8-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eafd8-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="eafd8-120">Remarks</span></span>

<span data-ttu-id="eafd8-121">Une instance [GroupedItems](groupeditems.md) se produira pour chaque groupe distinct dans le résultat.</span><span class="sxs-lookup"><span data-stu-id="eafd8-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="eafd8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="eafd8-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eafd8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eafd8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eafd8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eafd8-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eafd8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eafd8-125">Schema name</span></span>  <br/> |<span data-ttu-id="eafd8-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eafd8-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="eafd8-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eafd8-127">Validation file</span></span>  <br/> |<span data-ttu-id="eafd8-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eafd8-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eafd8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eafd8-129">Can be empty</span></span>  <br/> |<span data-ttu-id="eafd8-130">False</span><span class="sxs-lookup"><span data-stu-id="eafd8-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eafd8-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eafd8-131">See also</span></span>



[<span data-ttu-id="eafd8-132">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="eafd8-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="eafd8-133">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="eafd8-133">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

