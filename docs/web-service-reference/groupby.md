---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: L’élément GroupBy spécifie un regroupement pour les requêtes FindItem arbitraire.
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827753"
---
# <a name="groupby"></a><span data-ttu-id="ea9d5-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="ea9d5-103">GroupBy</span></span>

<span data-ttu-id="ea9d5-104">L’élément **GroupBy** spécifie un regroupement pour les requêtes FindItem arbitraire.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="ea9d5-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="ea9d5-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="ea9d5-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="ea9d5-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

 <span data-ttu-id="ea9d5-107">**GroupByType**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-107">**GroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea9d5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea9d5-108">Attributes and elements</span></span>

<span data-ttu-id="ea9d5-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea9d5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea9d5-110">Attributes</span></span>

|<span data-ttu-id="ea9d5-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-111">**Attribute**</span></span>|<span data-ttu-id="ea9d5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea9d5-113">**Order**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-113">**Order**</span></span> <br/> | <span data-ttu-id="ea9d5-114">Détermine l’ordre des groupes dans le tableau élément groupé qui est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="ea9d5-115">Cet attribut est de type SortDirectionType.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="ea9d5-116">Valeurs d’attribut ordre</span><span class="sxs-lookup"><span data-stu-id="ea9d5-116">Order attribute values</span></span>

|<span data-ttu-id="ea9d5-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-117">**Value**</span></span>|<span data-ttu-id="ea9d5-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea9d5-119">Croissant</span><span class="sxs-lookup"><span data-stu-id="ea9d5-119">Ascending</span></span>  <br/> |<span data-ttu-id="ea9d5-120">Les groupes sont triés par ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="ea9d5-121">Décroissant</span><span class="sxs-lookup"><span data-stu-id="ea9d5-121">Descending</span></span>  <br/> |<span data-ttu-id="ea9d5-122">Les groupes sont triés par ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ea9d5-123">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea9d5-123">Child elements</span></span>

|<span data-ttu-id="ea9d5-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-124">**Element**</span></span>|<span data-ttu-id="ea9d5-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea9d5-126">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ea9d5-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ea9d5-127">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ea9d5-128">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ea9d5-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ea9d5-129">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="ea9d5-130">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ea9d5-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ea9d5-131">Identifie les propriétés MAPI étendues pour obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="ea9d5-132">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="ea9d5-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="ea9d5-133">Représente le champ qui est utilisé pour déterminer l’ordre des groupes dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea9d5-134">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea9d5-134">Parent elements</span></span>

|<span data-ttu-id="ea9d5-135">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-135">**Element**</span></span>|<span data-ttu-id="ea9d5-136">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea9d5-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea9d5-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="ea9d5-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ea9d5-138">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="ea9d5-139">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="ea9d5-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea9d5-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea9d5-140">Remarks</span></span>

<span data-ttu-id="ea9d5-141">La réponse FindItem contient une collection de groupes.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="ea9d5-142">Chaque groupe contiendra tous les éléments ayant des valeurs de la propriété **GroupBy** correspondantes.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="ea9d5-143">La propriété qui détermine le groupement est identifiée dans l’élément [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="ea9d5-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="ea9d5-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ea9d5-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea9d5-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ea9d5-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea9d5-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ea9d5-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea9d5-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ea9d5-147">Schema Name</span></span>  <br/> |<span data-ttu-id="ea9d5-148">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ea9d5-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea9d5-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ea9d5-149">Validation File</span></span>  <br/> |<span data-ttu-id="ea9d5-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea9d5-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea9d5-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ea9d5-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea9d5-152">False</span><span class="sxs-lookup"><span data-stu-id="ea9d5-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea9d5-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea9d5-153">See also</span></span>

- [<span data-ttu-id="ea9d5-154">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="ea9d5-154">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="ea9d5-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ea9d5-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ea9d5-156">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="ea9d5-156">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

