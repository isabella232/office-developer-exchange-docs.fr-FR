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
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467017"
---
# <a name="indexedfielduri"></a><span data-ttu-id="fd848-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fd848-103">IndexedFieldURI</span></span>

<span data-ttu-id="fd848-104">L’élément **IndexedFieldURI** identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="fd848-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="fd848-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="fd848-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd848-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fd848-106">Attributes and elements</span></span>

<span data-ttu-id="fd848-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fd848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd848-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fd848-108">Attributes</span></span>

|<span data-ttu-id="fd848-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fd848-109">**Attribute**</span></span>|<span data-ttu-id="fd848-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd848-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd848-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="fd848-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="fd848-112">Identifie le dictionnaire qui contient le membre à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="fd848-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="fd848-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="fd848-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fd848-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="fd848-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="fd848-115">Identifie le membre du dictionnaire à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="fd848-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="fd848-116">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="fd848-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="fd848-117">Attribut FieldURI</span><span class="sxs-lookup"><span data-stu-id="fd848-117">FieldURI Attribute</span></span>

|<span data-ttu-id="fd848-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fd848-118">**Value**</span></span>|<span data-ttu-id="fd848-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd848-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd848-120">élément : InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="fd848-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="fd848-121">Représente l’en-tête de message d’un élément.</span><span class="sxs-lookup"><span data-stu-id="fd848-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="fd848-122">contacts : IMAddress</span><span class="sxs-lookup"><span data-stu-id="fd848-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="fd848-123">Représente l’adresse de messagerie instantanée d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-124">contacts : PhysicalAddress : rue</span><span class="sxs-lookup"><span data-stu-id="fd848-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="fd848-125">Représente l’adresse postale d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-126">contacts : PhysicalAddress : City</span><span class="sxs-lookup"><span data-stu-id="fd848-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="fd848-127">Représente la ville d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-128">contacts : PhysicalAddress : état</span><span class="sxs-lookup"><span data-stu-id="fd848-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="fd848-129">Représente l’état d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-130">contacts : PhysicalAddress : pays</span><span class="sxs-lookup"><span data-stu-id="fd848-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="fd848-131">Représente le pays/la région d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-132">contacts : PhysicalAddress : CodePostal</span><span class="sxs-lookup"><span data-stu-id="fd848-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="fd848-133">Représente le code postal d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-134">contacts : PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fd848-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="fd848-135">Représente le numéro de téléphone d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-136">contacts : EmailAddress</span><span class="sxs-lookup"><span data-stu-id="fd848-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="fd848-137">Représente l’adresse de messagerie d’un contact.</span><span class="sxs-lookup"><span data-stu-id="fd848-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="fd848-138">DistributionList : membres : membre</span><span class="sxs-lookup"><span data-stu-id="fd848-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="fd848-139">Représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="fd848-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fd848-140">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fd848-140">Child elements</span></span>

<span data-ttu-id="fd848-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fd848-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd848-142">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fd848-142">Parent elements</span></span>

|<span data-ttu-id="fd848-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd848-143">**Element**</span></span>|<span data-ttu-id="fd848-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd848-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd848-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="fd848-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="fd848-146">Identifie les propriétés supplémentaires à obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="fd848-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="fd848-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="fd848-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="fd848-148">Représente la propriété qui est utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé.</span><span class="sxs-lookup"><span data-stu-id="fd848-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="fd848-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="fd848-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="fd848-150">Spécifie un regroupement arbitraire pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="fd848-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd848-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="fd848-151">Remarks</span></span>

<span data-ttu-id="fd848-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd848-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd848-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fd848-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd848-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fd848-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd848-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fd848-155">Schema Name</span></span>  <br/> |<span data-ttu-id="fd848-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fd848-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd848-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fd848-157">Validation File</span></span>  <br/> |<span data-ttu-id="fd848-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd848-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd848-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fd848-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd848-160">False</span><span class="sxs-lookup"><span data-stu-id="fd848-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd848-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd848-161">See also</span></span>



- [<span data-ttu-id="fd848-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fd848-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

