---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: L’élément ItemChange, contient un identificateur d’élément et les mises à jour à appliquer à l’élément.
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459916"
---
# <a name="itemchange"></a><span data-ttu-id="4dd17-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="4dd17-103">ItemChange</span></span>

<span data-ttu-id="4dd17-104">L’élément **ItemChange,** contient un identificateur d’élément et les mises à jour à appliquer à l’élément.</span><span class="sxs-lookup"><span data-stu-id="4dd17-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
- [<span data-ttu-id="4dd17-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4dd17-105">UpdateItem</span></span>](updateitem.md) 
- [<span data-ttu-id="4dd17-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="4dd17-106">ItemChanges</span></span>](itemchanges.md)
- [<span data-ttu-id="4dd17-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="4dd17-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

<span data-ttu-id="4dd17-108">**ItemChangeType**</span><span class="sxs-lookup"><span data-stu-id="4dd17-108">**ItemChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4dd17-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4dd17-109">Attributes and elements</span></span>

<span data-ttu-id="4dd17-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4dd17-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dd17-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4dd17-111">Attributes</span></span>

<span data-ttu-id="4dd17-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4dd17-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dd17-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4dd17-113">Child elements</span></span>

|<span data-ttu-id="4dd17-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4dd17-114">**Element**</span></span>|<span data-ttu-id="4dd17-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="4dd17-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dd17-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="4dd17-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4dd17-117">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4dd17-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="4dd17-118">Cet élément est requis si l’élément [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) n’est pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="4dd17-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="4dd17-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="4dd17-120">Identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="4dd17-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="4dd17-121">Cet élément est requis s’il est utilisé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-121">This element is required if used.</span></span> <span data-ttu-id="4dd17-122">Cet élément est requis si l’élément [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) n’est pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="4dd17-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="4dd17-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="4dd17-124">Identifie un élément de la forme de base de récurrence en identifiant l’un de ses éléments d’occurrences associés.</span><span class="sxs-lookup"><span data-stu-id="4dd17-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="4dd17-125">Cet élément est requis s’il est utilisé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-125">This element is required if used.</span></span> <span data-ttu-id="4dd17-126">Cet élément est requis si l’élément [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) n’est pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="4dd17-127">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="4dd17-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="4dd17-128">Contient un tableau qui définit les modifications d’ajout, de définition et de suppression des propriétés d’élément.</span><span class="sxs-lookup"><span data-stu-id="4dd17-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="4dd17-129">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4dd17-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4dd17-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4dd17-130">Parent elements</span></span>

|<span data-ttu-id="4dd17-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4dd17-131">**Element**</span></span>|<span data-ttu-id="4dd17-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="4dd17-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dd17-133">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="4dd17-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="4dd17-134">Contient un tableau d’éléments [ItemChange,](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.</span><span class="sxs-lookup"><span data-stu-id="4dd17-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="4dd17-135">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4dd17-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4dd17-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="4dd17-136">Remarks</span></span>

<span data-ttu-id="4dd17-137">Un seul élément [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) peut être utilisé dans un élément **ItemChange,** .</span><span class="sxs-lookup"><span data-stu-id="4dd17-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="4dd17-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4dd17-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4dd17-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4dd17-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dd17-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4dd17-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4dd17-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4dd17-141">Schema Name</span></span>  <br/> |<span data-ttu-id="4dd17-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4dd17-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="4dd17-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4dd17-143">Validation File</span></span>  <br/> |<span data-ttu-id="4dd17-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4dd17-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4dd17-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4dd17-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="4dd17-146">False</span><span class="sxs-lookup"><span data-stu-id="4dd17-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4dd17-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4dd17-147">See also</span></span>

- [<span data-ttu-id="4dd17-148">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="4dd17-148">UpdateItem operation</span></span>](updateitem-operation.md)

