---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: L’élément IndexedFieldURI identifie les membres individuels d’un dictionnaire.
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827909"
---
# <a name="indexedfielduri"></a><span data-ttu-id="a1cba-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a1cba-103">IndexedFieldURI</span></span>

<span data-ttu-id="a1cba-104">L’élément **IndexedFieldURI** identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="a1cba-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="a1cba-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="a1cba-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1cba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a1cba-106">Attributes and elements</span></span>

<span data-ttu-id="a1cba-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a1cba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1cba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a1cba-108">Attributes</span></span>

|<span data-ttu-id="a1cba-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a1cba-109">**Attribute**</span></span>|<span data-ttu-id="a1cba-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a1cba-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1cba-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="a1cba-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="a1cba-112">Identifie le dictionnaire qui contient le membre à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="a1cba-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="a1cba-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="a1cba-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a1cba-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="a1cba-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="a1cba-115">Identifie le membre du dictionnaire à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="a1cba-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="a1cba-116">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="a1cba-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="a1cba-117">Attribut FieldURI</span><span class="sxs-lookup"><span data-stu-id="a1cba-117">FieldURI Attribute</span></span>

|<span data-ttu-id="a1cba-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a1cba-118">**Value**</span></span>|<span data-ttu-id="a1cba-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a1cba-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1cba-120">élément : InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="a1cba-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="a1cba-121">Représente l’en-tête de message d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a1cba-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="a1cba-122">contacts : ImAddress</span><span class="sxs-lookup"><span data-stu-id="a1cba-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="a1cba-123">Représente l’adresse d’un contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a1cba-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-124">contacts : PhysicalAddress:Street</span><span class="sxs-lookup"><span data-stu-id="a1cba-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="a1cba-125">Représente l’adresse d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-126">contacts : PhysicalAddress:City</span><span class="sxs-lookup"><span data-stu-id="a1cba-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="a1cba-127">Représente la ville d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-128">contacts : PhysicalAddress:State</span><span class="sxs-lookup"><span data-stu-id="a1cba-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="a1cba-129">Représente l’état d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-130">contacts : PhysicalAddress:Country</span><span class="sxs-lookup"><span data-stu-id="a1cba-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="a1cba-131">Représente la pays/la région d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-132">contacts : PhysicalAddress:PostalCode</span><span class="sxs-lookup"><span data-stu-id="a1cba-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="a1cba-133">Représente le code postal du contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-134">contacts : PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a1cba-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="a1cba-135">Représente le numéro de téléphone d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-136">contacts : EmailAddress</span><span class="sxs-lookup"><span data-stu-id="a1cba-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="a1cba-137">Représente l’adresse de messagerie d’un contact.</span><span class="sxs-lookup"><span data-stu-id="a1cba-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1cba-138">DistributionList:members:Member</span><span class="sxs-lookup"><span data-stu-id="a1cba-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="a1cba-139">Représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="a1cba-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a1cba-140">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a1cba-140">Child elements</span></span>

<span data-ttu-id="a1cba-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a1cba-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1cba-142">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a1cba-142">Parent elements</span></span>

|<span data-ttu-id="a1cba-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a1cba-143">**Element**</span></span>|<span data-ttu-id="a1cba-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="a1cba-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1cba-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="a1cba-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="a1cba-146">Identifie les propriétés supplémentaires pour obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="a1cba-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="a1cba-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="a1cba-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="a1cba-148">Représente la propriété qui est utilisée pour déterminer l’ordre des éléments regroupés pour un jeu de résultats FindItem groupé.</span><span class="sxs-lookup"><span data-stu-id="a1cba-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="a1cba-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="a1cba-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="a1cba-150">Spécifie un regroupement pour les requêtes FindItem arbitraire.</span><span class="sxs-lookup"><span data-stu-id="a1cba-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1cba-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="a1cba-151">Remarks</span></span>

<span data-ttu-id="a1cba-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1cba-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1cba-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a1cba-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1cba-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a1cba-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1cba-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a1cba-155">Schema Name</span></span>  <br/> |<span data-ttu-id="a1cba-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a1cba-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1cba-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a1cba-157">Validation File</span></span>  <br/> |<span data-ttu-id="a1cba-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a1cba-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1cba-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a1cba-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1cba-160">False</span><span class="sxs-lookup"><span data-stu-id="a1cba-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1cba-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a1cba-161">See also</span></span>



- [<span data-ttu-id="a1cba-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a1cba-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

