---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: L’élément AlternatePublicFolderItemId décrit un identificateur d’élément de dossier public à convertir en un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755202"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="34565-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="34565-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="34565-105">L’élément **AlternatePublicFolderItemId** décrit un identificateur d’élément de dossier public à convertir en un autre format d’identificateur.</span><span class="sxs-lookup"><span data-stu-id="34565-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="34565-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="34565-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="34565-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="34565-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="34565-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="34565-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="34565-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="34565-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="34565-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="34565-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34565-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34565-111">Attributes and elements</span></span>

<span data-ttu-id="34565-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34565-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34565-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="34565-113">Attributes</span></span>

|<span data-ttu-id="34565-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="34565-114">**Attribute**</span></span>|<span data-ttu-id="34565-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="34565-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34565-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="34565-116">FolderId</span></span>  <br/> |<span data-ttu-id="34565-117">Identifie le dossier public qui contient l’élément du dossier public.</span><span class="sxs-lookup"><span data-stu-id="34565-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="34565-118">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="34565-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="34565-119">Format</span><span class="sxs-lookup"><span data-stu-id="34565-119">Format</span></span>  <br/> |<span data-ttu-id="34565-120">Identifie le format qui décrit l’identificateur d’élément de dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="34565-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="34565-121">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="34565-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="34565-122">ItemId</span><span class="sxs-lookup"><span data-stu-id="34565-122">ItemId</span></span>  <br/> |<span data-ttu-id="34565-123">Identificateur de l’élément du dossier public à convertir.</span><span class="sxs-lookup"><span data-stu-id="34565-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="34565-124">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="34565-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="34565-125">Valeurs d’attribut de format</span><span class="sxs-lookup"><span data-stu-id="34565-125">Format attribute values</span></span>

|<span data-ttu-id="34565-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="34565-126">**Value**</span></span>|<span data-ttu-id="34565-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="34565-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34565-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="34565-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="34565-129">Décrit les identificateurs qui sont générées par les Services Web Exchange dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="34565-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="34565-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="34565-130">EwsId</span></span>  <br/> |<span data-ttu-id="34565-131">Décrit les identificateurs qui sont générées par les Services Web Exchange commençant par Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="34565-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="34565-132">Propriété EntryId</span><span class="sxs-lookup"><span data-stu-id="34565-132">EntryId</span></span>  <br/> |<span data-ttu-id="34565-133">Décrit les identificateurs MAPI, comme illustré à la propriété PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="34565-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="34565-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="34565-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="34565-135">Décrit une représentation de la propriété PR_ENTRYID codé en hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="34565-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="34565-136">Il s’agit du format des identificateurs d’événement de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="34565-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="34565-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="34565-137">StoreId</span></span>  <br/> |<span data-ttu-id="34565-138">Décrit les identificateurs de banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="34565-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="34565-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="34565-139">OwaId</span></span>  <br/> |<span data-ttu-id="34565-140">Décrit un identificateur d’Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="34565-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="34565-141">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34565-141">Child elements</span></span>

<span data-ttu-id="34565-142">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34565-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34565-143">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34565-143">Parent elements</span></span>

|<span data-ttu-id="34565-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34565-144">**Element**</span></span>|<span data-ttu-id="34565-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="34565-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34565-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="34565-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="34565-147">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="34565-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="34565-148">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="34565-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34565-149">Remarques</span><span class="sxs-lookup"><span data-stu-id="34565-149">Remarks</span></span>

<span data-ttu-id="34565-150">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="34565-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34565-151">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34565-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34565-152">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34565-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34565-153">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34565-153">Schema Name</span></span>  <br/> |<span data-ttu-id="34565-154">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="34565-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="34565-155">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34565-155">Validation File</span></span>  <br/> |<span data-ttu-id="34565-156">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="34565-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34565-157">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34565-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="34565-158">True</span><span class="sxs-lookup"><span data-stu-id="34565-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34565-159">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34565-159">See also</span></span>

- [<span data-ttu-id="34565-160">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="34565-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="34565-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="34565-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="34565-162">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="34565-162">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

