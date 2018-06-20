---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: L’élément RecurringMasterItemId identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829015"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="e9ffe-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="e9ffe-103">RecurringMasterItemId</span></span>

<span data-ttu-id="e9ffe-104">L’élément **RecurringMasterItemId** identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="e9ffe-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9ffe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9ffe-106">Attributes and elements</span></span>

<span data-ttu-id="e9ffe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9ffe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9ffe-108">Attributes</span></span>

|<span data-ttu-id="e9ffe-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-109">**Attribute**</span></span>|<span data-ttu-id="e9ffe-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9ffe-111">**ID d’occurrence**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="e9ffe-112">Identifie une seule occurrence d’un rendez-vous périodique.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="e9ffe-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e9ffe-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="e9ffe-115">Identifie une version spécifique d’une seule occurrence d’un rendez-vous périodique.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="e9ffe-116">En outre, le rendez-vous périodique est également identifié, car elle et l’occurrence contiendra la même clé change.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="e9ffe-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e9ffe-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9ffe-118">Child elements</span></span>

<span data-ttu-id="e9ffe-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9ffe-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9ffe-120">Parent elements</span></span>

|<span data-ttu-id="e9ffe-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-121">**Element**</span></span>|<span data-ttu-id="e9ffe-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9ffe-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9ffe-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="e9ffe-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="e9ffe-124">Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e9ffe-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="e9ffe-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="e9ffe-126">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="e9ffe-127">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e9ffe-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="e9ffe-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="e9ffe-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="e9ffe-129">Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="e9ffe-130">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="e9ffe-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9ffe-131">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e9ffe-131">Text value</span></span>

<span data-ttu-id="e9ffe-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9ffe-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="e9ffe-133">Remarks</span></span>

<span data-ttu-id="e9ffe-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="e9ffe-135">Exemple</span><span class="sxs-lookup"><span data-stu-id="e9ffe-135">Example</span></span>

<span data-ttu-id="e9ffe-136">L’exemple suivant identifie le rendez-vous périodique en identifiant une de ses occurrences avec l’identificateur 56lkjh6.</span><span class="sxs-lookup"><span data-stu-id="e9ffe-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="e9ffe-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9ffe-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9ffe-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9ffe-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9ffe-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9ffe-139">Schema Name</span></span>  <br/> |<span data-ttu-id="e9ffe-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e9ffe-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9ffe-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9ffe-141">Validation File</span></span>  <br/> |<span data-ttu-id="e9ffe-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9ffe-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9ffe-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9ffe-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9ffe-144">False</span><span class="sxs-lookup"><span data-stu-id="e9ffe-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9ffe-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9ffe-145">See also</span></span>

- [<span data-ttu-id="e9ffe-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="e9ffe-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="e9ffe-147">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="e9ffe-147">FindConversation operation</span></span>](findconversation-operation.md)

