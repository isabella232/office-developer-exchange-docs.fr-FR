---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: L’élément StandardGroupBy représente les mécanismes de regroupement et d’agrégation standard d’une opération groupée FindItem.
ms.openlocfilehash: 3e135feba322979de3d66d5a45d423654ccc9100
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467556"
---
# <a name="standardgroupby"></a><span data-ttu-id="4fe90-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="4fe90-103">StandardGroupBy</span></span>

<span data-ttu-id="4fe90-104">L’élément **StandardGroupBy** représente les mécanismes de regroupement et d’agrégation standard d’une opération groupée FindItem.</span><span class="sxs-lookup"><span data-stu-id="4fe90-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="4fe90-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="4fe90-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="4fe90-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="4fe90-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="4fe90-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="4fe90-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="4fe90-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="4fe90-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fe90-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4fe90-109">Attributes and elements</span></span>

<span data-ttu-id="4fe90-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4fe90-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe90-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4fe90-111">Attributes</span></span>

<span data-ttu-id="4fe90-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4fe90-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fe90-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4fe90-113">Child elements</span></span>

<span data-ttu-id="4fe90-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4fe90-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fe90-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4fe90-115">Parent elements</span></span>

|<span data-ttu-id="4fe90-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4fe90-116">**Element**</span></span>|<span data-ttu-id="4fe90-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4fe90-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe90-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="4fe90-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="4fe90-119">Fournit des regroupements standard pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="4fe90-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fe90-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4fe90-120">Text value</span></span>

<span data-ttu-id="4fe90-121">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="4fe90-121">A text value is required.</span></span> <span data-ttu-id="4fe90-122">La seule valeur qui peut être utilisée pour cet élément est **ConversationTopic**.</span><span class="sxs-lookup"><span data-stu-id="4fe90-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="4fe90-123">**ConversationTopic** Groups par message : ConversationTopic et Aggregates on Item : DateTimeReceived (maximum).</span><span class="sxs-lookup"><span data-stu-id="4fe90-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="4fe90-124">Pour plus d’informations sur l’agrégation, voir [AggregateOn](aggregateon.md).</span><span class="sxs-lookup"><span data-stu-id="4fe90-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4fe90-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="4fe90-125">Remarks</span></span>

<span data-ttu-id="4fe90-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4fe90-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fe90-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4fe90-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe90-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4fe90-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fe90-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4fe90-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4fe90-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4fe90-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fe90-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4fe90-131">Validation File</span></span>  <br/> |<span data-ttu-id="4fe90-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fe90-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fe90-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4fe90-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fe90-134">False</span><span class="sxs-lookup"><span data-stu-id="4fe90-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fe90-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4fe90-135">See also</span></span>



[<span data-ttu-id="4fe90-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="4fe90-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="4fe90-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="4fe90-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="4fe90-138">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="4fe90-138">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

