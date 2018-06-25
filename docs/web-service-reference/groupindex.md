---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: L’élément GroupIndex représente la valeur de la propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments dans un appel de l’opération FindItem actuel.
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827762"
---
# <a name="groupindex"></a><span data-ttu-id="d7432-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="d7432-103">GroupIndex</span></span>

<span data-ttu-id="d7432-104">L’élément **GroupIndex** représente la valeur de la propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments dans un appel [FindItem opération](finditem-operation.md) en cours.</span><span class="sxs-lookup"><span data-stu-id="d7432-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="d7432-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="d7432-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="d7432-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7432-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="d7432-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7432-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="d7432-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d7432-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="d7432-109">Groupes</span><span class="sxs-lookup"><span data-stu-id="d7432-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="d7432-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d7432-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="d7432-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="d7432-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="d7432-112">**string**</span><span class="sxs-lookup"><span data-stu-id="d7432-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7432-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d7432-113">Attributes and elements</span></span>

<span data-ttu-id="d7432-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d7432-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7432-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="d7432-115">Attributes</span></span>

<span data-ttu-id="d7432-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d7432-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7432-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d7432-117">Child elements</span></span>

<span data-ttu-id="d7432-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d7432-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7432-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d7432-119">Parent elements</span></span>

|<span data-ttu-id="d7432-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7432-120">**Element**</span></span>|<span data-ttu-id="d7432-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7432-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7432-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d7432-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="d7432-123">Représente une collection d’éléments qui sont le résultat d’une [opération FindItem](finditem-operation.md) groupée appeler.</span><span class="sxs-lookup"><span data-stu-id="d7432-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="d7432-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d7432-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7432-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d7432-125">Text value</span></span>

<span data-ttu-id="d7432-126">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d7432-126">A text value is required.</span></span> <span data-ttu-id="d7432-127">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="d7432-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d7432-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="d7432-128">Remarks</span></span>

<span data-ttu-id="d7432-129">Cet élément ne se produit dans une réponse de [l’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7432-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="d7432-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d7432-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7432-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d7432-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7432-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d7432-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7432-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d7432-133">Schema name</span></span>  <br/> |<span data-ttu-id="d7432-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d7432-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7432-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d7432-135">Validation file</span></span>  <br/> |<span data-ttu-id="d7432-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d7432-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7432-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d7432-137">Can be empty</span></span>  <br/> |<span data-ttu-id="d7432-138">False</span><span class="sxs-lookup"><span data-stu-id="d7432-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7432-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d7432-139">See also</span></span>



[<span data-ttu-id="d7432-140">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="d7432-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="d7432-141">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="d7432-141">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

