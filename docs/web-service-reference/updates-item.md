---
title: Mises à jour (élément)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: L’élément updates contient un ensemble d’éléments qui définissent les modifications apportées par l’ajout, la définition et la suppression aux propriétés des éléments.
ms.openlocfilehash: 6902ea4d3d3d9adc074745d5642cdfa6d91a9163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456352"
---
# <a name="updates-item"></a><span data-ttu-id="3a141-103">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="3a141-103">Updates (Item)</span></span>

<span data-ttu-id="3a141-104">L’élément **updates** contient un ensemble d’éléments qui définissent les modifications apportées par l’ajout, la définition et la suppression aux propriétés des éléments.</span><span class="sxs-lookup"><span data-stu-id="3a141-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="3a141-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="3a141-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="3a141-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="3a141-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="3a141-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="3a141-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="3a141-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="3a141-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="3a141-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="3a141-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3a141-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3a141-110">Attributes and elements</span></span>

<span data-ttu-id="3a141-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3a141-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a141-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3a141-112">Attributes</span></span>

<span data-ttu-id="3a141-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3a141-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a141-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3a141-114">Child elements</span></span>

|<span data-ttu-id="3a141-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a141-115">**Element**</span></span>|<span data-ttu-id="3a141-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a141-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a141-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="3a141-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="3a141-118">Représente les données à ajouter à une propriété unique d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3a141-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3a141-119">SetItemField</span><span class="sxs-lookup"><span data-stu-id="3a141-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="3a141-120">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3a141-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3a141-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="3a141-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="3a141-122">Représente une opération permettant de supprimer une propriété donnée d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3a141-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a141-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3a141-123">Parent elements</span></span>

|<span data-ttu-id="3a141-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a141-124">**Element**</span></span>|<span data-ttu-id="3a141-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a141-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a141-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="3a141-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="3a141-127">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="3a141-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="3a141-128">Voici l’expression XPath de cet élément :`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="3a141-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3a141-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="3a141-129">Remarks</span></span>

<span data-ttu-id="3a141-130">Les mises à jour définies par cet élément sont effectuées sur l’élément qui est identifié par les éléments [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="3a141-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="3a141-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3a141-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a141-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3a141-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a141-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3a141-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a141-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3a141-134">Schema Name</span></span>  <br/> |<span data-ttu-id="3a141-135">schéma de types</span><span class="sxs-lookup"><span data-stu-id="3a141-135">types schema</span></span>  <br/> |
|<span data-ttu-id="3a141-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3a141-136">Validation File</span></span>  <br/> |<span data-ttu-id="3a141-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3a141-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a141-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3a141-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a141-139">False</span><span class="sxs-lookup"><span data-stu-id="3a141-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a141-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3a141-140">See also</span></span>

- [<span data-ttu-id="3a141-141">Opération UpdateItem</span><span class="sxs-lookup"><span data-stu-id="3a141-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="3a141-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3a141-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

