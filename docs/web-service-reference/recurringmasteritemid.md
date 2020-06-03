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
description: L’élément RecurringMasterItemId identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529881"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="4d2ed-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="4d2ed-103">RecurringMasterItemId</span></span>

<span data-ttu-id="4d2ed-104">L’élément **RecurringMasterItemId** identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="4d2ed-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d2ed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d2ed-106">Attributes and elements</span></span>

<span data-ttu-id="4d2ed-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d2ed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d2ed-108">Attributes</span></span>

|<span data-ttu-id="4d2ed-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-109">**Attribute**</span></span>|<span data-ttu-id="4d2ed-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d2ed-111">**OccurrenceId**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="4d2ed-112">Identifie une seule occurrence d’un élément maître périodique.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="4d2ed-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4d2ed-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="4d2ed-115">Identifie une version spécifique d’une occurrence d’un élément maître périodique.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="4d2ed-116">En outre, l’élément de gabarit périodique est également identifié, car il et la seule occurrence contiendront la même clé de modification.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="4d2ed-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4d2ed-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d2ed-118">Child elements</span></span>

<span data-ttu-id="4d2ed-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d2ed-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d2ed-120">Parent elements</span></span>

|<span data-ttu-id="4d2ed-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-121">**Element**</span></span>|<span data-ttu-id="4d2ed-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d2ed-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d2ed-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="4d2ed-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="4d2ed-124">Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4d2ed-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="4d2ed-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="4d2ed-126">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="4d2ed-127">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4d2ed-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="4d2ed-128">ItemIds</span><span class="sxs-lookup"><span data-stu-id="4d2ed-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="4d2ed-129">Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="4d2ed-130">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4d2ed-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d2ed-131">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4d2ed-131">Text value</span></span>

<span data-ttu-id="4d2ed-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4d2ed-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d2ed-133">Remarks</span></span>

<span data-ttu-id="4d2ed-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="4d2ed-135">Exemple</span><span class="sxs-lookup"><span data-stu-id="4d2ed-135">Example</span></span>

<span data-ttu-id="4d2ed-136">L’exemple suivant identifie l’élément de forme de base périodique en identifiant l’une de ses occurrences à l’aide de l’identificateur 56lkjh6.</span><span class="sxs-lookup"><span data-stu-id="4d2ed-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="4d2ed-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d2ed-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d2ed-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d2ed-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d2ed-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d2ed-139">Schema Name</span></span>  <br/> |<span data-ttu-id="4d2ed-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4d2ed-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d2ed-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d2ed-141">Validation File</span></span>  <br/> |<span data-ttu-id="4d2ed-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d2ed-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d2ed-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d2ed-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d2ed-144">False</span><span class="sxs-lookup"><span data-stu-id="4d2ed-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d2ed-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d2ed-145">See also</span></span>

- [<span data-ttu-id="4d2ed-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="4d2ed-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="4d2ed-147">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="4d2ed-147">FindConversation operation</span></span>](findconversation-operation.md)

