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
description: L’élément GroupIndex représente la valeur de propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments en cours dans un appel d’opération FindItem.
ms.openlocfilehash: 05f303be92885a15dddf85c85251af04910d835c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530267"
---
# <a name="groupindex"></a><span data-ttu-id="0ed4d-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="0ed4d-103">GroupIndex</span></span>

<span data-ttu-id="0ed4d-104">L’élément **GroupIndex** représente la valeur de propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments en cours dans un appel d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ed4d-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="0ed4d-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="0ed4d-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="0ed4d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ed4d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="0ed4d-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ed4d-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="0ed4d-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="0ed4d-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="0ed4d-109">Groups</span><span class="sxs-lookup"><span data-stu-id="0ed4d-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="0ed4d-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="0ed4d-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="0ed4d-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="0ed4d-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="0ed4d-112">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="0ed4d-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ed4d-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ed4d-113">Attributes and elements</span></span>

<span data-ttu-id="0ed4d-114">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ed4d-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ed4d-115">Attributes</span></span>

<span data-ttu-id="0ed4d-116">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ed4d-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ed4d-117">Child elements</span></span>

<span data-ttu-id="0ed4d-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ed4d-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ed4d-119">Parent elements</span></span>

|<span data-ttu-id="0ed4d-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ed4d-120">**Element**</span></span>|<span data-ttu-id="0ed4d-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ed4d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ed4d-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="0ed4d-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="0ed4d-123">Représente une collection d’éléments qui sont le résultat d’un appel d' [opération FindItem](finditem-operation.md) groupé.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="0ed4d-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="0ed4d-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ed4d-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0ed4d-125">Text value</span></span>

<span data-ttu-id="0ed4d-126">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-126">A text value is required.</span></span> <span data-ttu-id="0ed4d-127">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ed4d-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ed4d-128">Remarks</span></span>

<span data-ttu-id="0ed4d-129">Cet élément ne se produit que dans une réponse d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ed4d-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="0ed4d-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0ed4d-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ed4d-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ed4d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ed4d-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ed4d-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ed4d-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ed4d-133">Schema name</span></span>  <br/> |<span data-ttu-id="0ed4d-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0ed4d-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ed4d-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ed4d-135">Validation file</span></span>  <br/> |<span data-ttu-id="0ed4d-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ed4d-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ed4d-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ed4d-137">Can be empty</span></span>  <br/> |<span data-ttu-id="0ed4d-138">False</span><span class="sxs-lookup"><span data-stu-id="0ed4d-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ed4d-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ed4d-139">See also</span></span>



[<span data-ttu-id="0ed4d-140">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="0ed4d-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="0ed4d-141">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="0ed4d-141">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

