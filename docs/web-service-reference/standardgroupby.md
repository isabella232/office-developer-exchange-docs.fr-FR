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
description: L’élément StandardGroupBy représente la norme groupement et agrégation des mécanismes d’une opération FindItem groupée.
ms.openlocfilehash: 8e2ec72a79ebafc2e5757d6dcebb27c0c53ec0b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829542"
---
# <a name="standardgroupby"></a><span data-ttu-id="d04f3-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="d04f3-103">StandardGroupBy</span></span>

<span data-ttu-id="d04f3-104">L’élément **StandardGroupBy** représente la norme groupement et agrégation des mécanismes d’une opération FindItem groupée.</span><span class="sxs-lookup"><span data-stu-id="d04f3-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="d04f3-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="d04f3-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="d04f3-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="d04f3-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="d04f3-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="d04f3-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="d04f3-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="d04f3-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d04f3-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d04f3-109">Attributes and elements</span></span>

<span data-ttu-id="d04f3-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d04f3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d04f3-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="d04f3-111">Attributes</span></span>

<span data-ttu-id="d04f3-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d04f3-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d04f3-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d04f3-113">Child elements</span></span>

<span data-ttu-id="d04f3-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d04f3-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d04f3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d04f3-115">Parent elements</span></span>

|<span data-ttu-id="d04f3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d04f3-116">**Element**</span></span>|<span data-ttu-id="d04f3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d04f3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d04f3-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="d04f3-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="d04f3-119">Fournit des regroupements standards pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="d04f3-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d04f3-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d04f3-120">Text value</span></span>

<span data-ttu-id="d04f3-121">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d04f3-121">A text value is required.</span></span> <span data-ttu-id="d04f3-122">La seule valeur qui peut être utilisée pour cet élément est **ConversationTopic**.</span><span class="sxs-lookup"><span data-stu-id="d04f3-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="d04f3-123">Groupes **ConversationTopic** par message : ConversationTopic et agrégats sur élément : DateTimeReceived (maximum).</span><span class="sxs-lookup"><span data-stu-id="d04f3-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="d04f3-124">Pour plus d’informations sur l’agrégation, voir [AggregateOn](aggregateon.md).</span><span class="sxs-lookup"><span data-stu-id="d04f3-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d04f3-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="d04f3-125">Remarks</span></span>

<span data-ttu-id="d04f3-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d04f3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d04f3-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d04f3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d04f3-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d04f3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d04f3-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d04f3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d04f3-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d04f3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d04f3-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d04f3-131">Validation File</span></span>  <br/> |<span data-ttu-id="d04f3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d04f3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d04f3-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d04f3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d04f3-134">False</span><span class="sxs-lookup"><span data-stu-id="d04f3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d04f3-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d04f3-135">See also</span></span>



[<span data-ttu-id="d04f3-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="d04f3-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="d04f3-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="d04f3-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="d04f3-138">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="d04f3-138">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

