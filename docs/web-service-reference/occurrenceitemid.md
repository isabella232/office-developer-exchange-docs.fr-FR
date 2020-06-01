---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: L’élément OccurrenceItemId identifie une seule occurrence d’un élément périodique.
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468375"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="243ad-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="243ad-103">OccurrenceItemId</span></span>

<span data-ttu-id="243ad-104">L’élément **OccurrenceItemId** identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="243ad-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="243ad-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="243ad-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="243ad-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="243ad-106">Attributes and elements</span></span>

<span data-ttu-id="243ad-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="243ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="243ad-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="243ad-108">Attributes</span></span>

|<span data-ttu-id="243ad-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="243ad-109">**Attribute**</span></span>|<span data-ttu-id="243ad-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="243ad-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="243ad-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="243ad-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="243ad-112">Identifie le masque périodique d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="243ad-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="243ad-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="243ad-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="243ad-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="243ad-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="243ad-115">Identifie une version spécifique de l’occurrence de la page maître périodique ou d’un élément.</span><span class="sxs-lookup"><span data-stu-id="243ad-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="243ad-116">Si la forme de base périodique ou l’une de ses occurrences change, le **ChangeKey** change.</span><span class="sxs-lookup"><span data-stu-id="243ad-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="243ad-117">Le **ChangeKey** est le même pour le masque périodique et toutes les occurrences.</span><span class="sxs-lookup"><span data-stu-id="243ad-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="243ad-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="243ad-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="243ad-119">Identifie l’index de l’occurrence de l’élément.</span><span class="sxs-lookup"><span data-stu-id="243ad-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="243ad-120">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="243ad-120">This attribute is required.</span></span> <span data-ttu-id="243ad-121">Cette valeur représente un entier.</span><span class="sxs-lookup"><span data-stu-id="243ad-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="243ad-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="243ad-122">Child elements</span></span>

<span data-ttu-id="243ad-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="243ad-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="243ad-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="243ad-124">Parent elements</span></span>

|<span data-ttu-id="243ad-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="243ad-125">**Element**</span></span>|<span data-ttu-id="243ad-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="243ad-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="243ad-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="243ad-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="243ad-128">Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="243ad-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="243ad-129">ItemIds</span><span class="sxs-lookup"><span data-stu-id="243ad-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="243ad-130">Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="243ad-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="243ad-131">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="243ad-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="243ad-132">**Remarque**: l’opération [MoveItem](moveitem-operation.md) et l' [opération CopyItem](copyitem-operation.md) fonctionnent uniquement avec des éléments de calendrier uniques et des éléments de forme de base périodiques.</span><span class="sxs-lookup"><span data-stu-id="243ad-132">**NOTE**: [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="243ad-133">Les occurrences d’élément ne sont pas valides avec ces opérations.</span><span class="sxs-lookup"><span data-stu-id="243ad-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="243ad-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="243ad-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="243ad-135">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="243ad-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="243ad-136">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="243ad-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="243ad-137">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="243ad-137">Text value</span></span>

<span data-ttu-id="243ad-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="243ad-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="243ad-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="243ad-139">Remarks</span></span>

<span data-ttu-id="243ad-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="243ad-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="243ad-141">Exemple</span><span class="sxs-lookup"><span data-stu-id="243ad-141">Example</span></span>

<span data-ttu-id="243ad-142">L’exemple suivant identifie la quatrième occurrence d’un élément périodique ayant l’identité 34vswe4.</span><span class="sxs-lookup"><span data-stu-id="243ad-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="243ad-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="243ad-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="243ad-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="243ad-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="243ad-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="243ad-145">Schema Name</span></span>  <br/> |<span data-ttu-id="243ad-146">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="243ad-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="243ad-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="243ad-147">Validation File</span></span>  <br/> |<span data-ttu-id="243ad-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="243ad-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="243ad-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="243ad-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="243ad-150">False</span><span class="sxs-lookup"><span data-stu-id="243ad-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="243ad-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="243ad-151">See also</span></span>

- [<span data-ttu-id="243ad-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="243ad-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="243ad-153">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="243ad-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="243ad-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="243ad-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

