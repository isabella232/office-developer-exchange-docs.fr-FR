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
description: L’élément de mises à jour contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément.
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838914"
---
# <a name="updates-item"></a><span data-ttu-id="d86ad-103">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="d86ad-103">Updates (Item)</span></span>

<span data-ttu-id="d86ad-104">L’élément de **mises à jour** contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="d86ad-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="d86ad-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d86ad-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="d86ad-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d86ad-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="d86ad-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d86ad-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="d86ad-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="d86ad-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="d86ad-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="d86ad-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d86ad-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d86ad-110">Attributes and elements</span></span>

<span data-ttu-id="d86ad-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d86ad-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d86ad-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d86ad-112">Attributes</span></span>

<span data-ttu-id="d86ad-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d86ad-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d86ad-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d86ad-114">Child elements</span></span>

|<span data-ttu-id="d86ad-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d86ad-115">**Element**</span></span>|<span data-ttu-id="d86ad-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d86ad-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d86ad-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d86ad-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="d86ad-118">Représente les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d86ad-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d86ad-119">SetItemField</span><span class="sxs-lookup"><span data-stu-id="d86ad-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="d86ad-120">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d86ad-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d86ad-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="d86ad-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="d86ad-122">Représente une opération de suppression d’une propriété donnée d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d86ad-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d86ad-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d86ad-123">Parent elements</span></span>

|<span data-ttu-id="d86ad-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d86ad-124">**Element**</span></span>|<span data-ttu-id="d86ad-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="d86ad-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d86ad-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d86ad-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="d86ad-127">Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="d86ad-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="d86ad-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="d86ad-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d86ad-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="d86ad-129">Remarks</span></span>

<span data-ttu-id="d86ad-130">Les mises à jour qui sont définies par cet élément sont effectuées sur l’élément identifié par les éléments [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) .</span><span class="sxs-lookup"><span data-stu-id="d86ad-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="d86ad-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d86ad-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d86ad-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d86ad-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d86ad-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d86ad-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d86ad-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d86ad-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d86ad-135">schéma de types</span><span class="sxs-lookup"><span data-stu-id="d86ad-135">types schema</span></span>  <br/> |
|<span data-ttu-id="d86ad-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d86ad-136">Validation File</span></span>  <br/> |<span data-ttu-id="d86ad-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d86ad-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d86ad-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d86ad-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d86ad-139">False</span><span class="sxs-lookup"><span data-stu-id="d86ad-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d86ad-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d86ad-140">See also</span></span>

- [<span data-ttu-id="d86ad-141">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d86ad-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="d86ad-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d86ad-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

