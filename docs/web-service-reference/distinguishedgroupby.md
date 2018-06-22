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
description: L’élément DistinguishedGroupBy fournit des regroupements standards pour les requêtes FindItem.
ms.openlocfilehash: 0635366447675bf28dedf3af4f7d76094ee5e0a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756013"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="6b6f2-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="6b6f2-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="6b6f2-104">L’élément **DistinguishedGroupBy** fournit des regroupements standards pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="6b6f2-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="6b6f2-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="6b6f2-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="6b6f2-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="6b6f2-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="6b6f2-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b6f2-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6b6f2-108">Attributes and elements</span></span>

<span data-ttu-id="6b6f2-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b6f2-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6b6f2-110">Attributes</span></span>

<span data-ttu-id="6b6f2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b6f2-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6b6f2-112">Child elements</span></span>

|<span data-ttu-id="6b6f2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b6f2-113">**Element**</span></span>|<span data-ttu-id="6b6f2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b6f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b6f2-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="6b6f2-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="6b6f2-116">Représente la norme groupement et agrégation des mécanismes d’une opération FindItem groupée.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b6f2-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6b6f2-117">Parent elements</span></span>

|<span data-ttu-id="6b6f2-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b6f2-118">**Element**</span></span>|<span data-ttu-id="6b6f2-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b6f2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b6f2-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="6b6f2-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="6b6f2-121">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="6b6f2-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="6b6f2-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b6f2-123">Note</span><span class="sxs-lookup"><span data-stu-id="6b6f2-123">Remarks</span></span>

<span data-ttu-id="6b6f2-124">L’élément **DistinguishedGroupBy** peut être ajouté à une opération FindItem lorsque les résultats doivent provenir sauvegardées regroupées et lorsque un des groupes standards remplit les conditions de regroupement.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="6b6f2-125">Si l’élément [GroupBy](groupby.md) ni l’élément **DistinguishedGroupBy** est spécifié, FindItem résultats seront reviendrons dissociées.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="6b6f2-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6b6f2-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b6f2-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6b6f2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b6f2-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6b6f2-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b6f2-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6b6f2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6b6f2-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6b6f2-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b6f2-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6b6f2-131">Validation File</span></span>  <br/> |<span data-ttu-id="6b6f2-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b6f2-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b6f2-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6b6f2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b6f2-134">False</span><span class="sxs-lookup"><span data-stu-id="6b6f2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b6f2-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b6f2-135">See also</span></span>

- [<span data-ttu-id="6b6f2-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="6b6f2-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="6b6f2-137">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="6b6f2-137">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

