---
title: DistinguishedGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: L’élément DistinguishedGroupBy fournit des regroupements standard pour les requêtes FindItem.
ms.openlocfilehash: 004613d55419a19f69e960203ae13d8d906b74c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463138"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="722af-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="722af-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="722af-104">L’élément **DistinguishedGroupBy** fournit des regroupements standard pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="722af-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="722af-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="722af-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="722af-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="722af-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="722af-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="722af-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="722af-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="722af-108">Attributes and elements</span></span>

<span data-ttu-id="722af-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="722af-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="722af-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="722af-110">Attributes</span></span>

<span data-ttu-id="722af-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="722af-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="722af-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="722af-112">Child elements</span></span>

|<span data-ttu-id="722af-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="722af-113">**Element**</span></span>|<span data-ttu-id="722af-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="722af-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="722af-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="722af-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="722af-116">Représente le regroupement standard et les mécanismes d’agrégation pour une opération FindItem groupée.</span><span class="sxs-lookup"><span data-stu-id="722af-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="722af-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="722af-117">Parent elements</span></span>

|<span data-ttu-id="722af-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="722af-118">**Element**</span></span>|<span data-ttu-id="722af-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="722af-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="722af-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="722af-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="722af-121">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="722af-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="722af-122">Voici l’expression XPath de cet élément :`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="722af-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="722af-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="722af-123">Remarks</span></span>

<span data-ttu-id="722af-124">L’élément **DistinguishedGroupBy** peut être ajouté à une opération FindItem lorsque les résultats doivent être regroupés et lorsqu’un des groupes standard répond aux exigences de regroupement.</span><span class="sxs-lookup"><span data-stu-id="722af-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="722af-125">Si ni l’élément **DistinguishedGroupBy** ni l’élément [GroupBy](groupby.md) ne sont spécifiés, les résultats de FindItem seront renvoyés non groupés.</span><span class="sxs-lookup"><span data-stu-id="722af-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="722af-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="722af-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="722af-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="722af-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="722af-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="722af-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="722af-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="722af-129">Schema Name</span></span>  <br/> |<span data-ttu-id="722af-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="722af-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="722af-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="722af-131">Validation File</span></span>  <br/> |<span data-ttu-id="722af-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="722af-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="722af-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="722af-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="722af-134">False</span><span class="sxs-lookup"><span data-stu-id="722af-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="722af-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="722af-135">See also</span></span>

- [<span data-ttu-id="722af-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="722af-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="722af-137">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="722af-137">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

