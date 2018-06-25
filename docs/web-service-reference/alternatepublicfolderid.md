---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: L’élément AlternatePublicFolderId décrit un identificateur de dossier public à convertir en un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755203"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="19099-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="19099-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="19099-105">L’élément **AlternatePublicFolderId** décrit un identificateur de dossier public à convertir en un autre format d’identificateur.</span><span class="sxs-lookup"><span data-stu-id="19099-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="19099-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="19099-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="19099-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="19099-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="19099-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="19099-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="19099-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="19099-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="19099-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="19099-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19099-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19099-111">Attributes and elements</span></span>

<span data-ttu-id="19099-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19099-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19099-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="19099-113">Attributes</span></span>

|<span data-ttu-id="19099-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="19099-114">**Attribute**</span></span>|<span data-ttu-id="19099-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="19099-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19099-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="19099-116">FolderId</span></span>  <br/> |<span data-ttu-id="19099-117">Contient l’identificateur de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="19099-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="19099-118">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="19099-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="19099-119">Format</span><span class="sxs-lookup"><span data-stu-id="19099-119">Format</span></span>  <br/> |<span data-ttu-id="19099-120">Identifie le format qui décrit l’identificateur de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="19099-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="19099-121">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="19099-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="19099-122">Attribut de format</span><span class="sxs-lookup"><span data-stu-id="19099-122">Format attribute</span></span>

|<span data-ttu-id="19099-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="19099-123">**Value**</span></span>|<span data-ttu-id="19099-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="19099-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19099-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="19099-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="19099-126">Décrit les identificateurs qui sont générées par les Services Web Exchange dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="19099-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="19099-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="19099-127">EwsId</span></span>  <br/> |<span data-ttu-id="19099-128">Décrit les identificateurs qui sont générées par les Services Web Exchange commençant par Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="19099-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="19099-129">Propriété EntryId</span><span class="sxs-lookup"><span data-stu-id="19099-129">EntryId</span></span>  <br/> |<span data-ttu-id="19099-130">Décrit les identificateurs MAPI, comme illustré à la propriété PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="19099-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="19099-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="19099-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="19099-132">Décrit une représentation de la propriété PR_ENTRYID codé en hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="19099-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="19099-133">Il s’agit du format des identificateurs d’événement de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="19099-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="19099-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="19099-134">StoreId</span></span>  <br/> |<span data-ttu-id="19099-135">Décrit les identificateurs de banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="19099-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="19099-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="19099-136">OwaId</span></span>  <br/> |<span data-ttu-id="19099-137">Décrit un identificateur d’Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="19099-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="19099-138">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19099-138">Child elements</span></span>

<span data-ttu-id="19099-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19099-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19099-140">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19099-140">Parent elements</span></span>

|<span data-ttu-id="19099-141">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19099-141">**Element**</span></span>|<span data-ttu-id="19099-142">**Description**</span><span class="sxs-lookup"><span data-stu-id="19099-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19099-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="19099-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="19099-144">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="19099-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="19099-145">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="19099-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="19099-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="19099-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19099-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="19099-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19099-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="19099-148">Schema Name</span></span>  <br/> |<span data-ttu-id="19099-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="19099-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="19099-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="19099-150">Validation File</span></span>  <br/> |<span data-ttu-id="19099-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19099-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19099-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="19099-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="19099-153">True</span><span class="sxs-lookup"><span data-stu-id="19099-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19099-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="19099-154">See also</span></span>

- [<span data-ttu-id="19099-155">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="19099-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="19099-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="19099-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="19099-157">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="19099-157">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

