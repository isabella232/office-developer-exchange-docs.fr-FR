---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: L’élément AlternateId décrit un identificateur pour convertir dans une requête et les résultats d’un identificateur converti dans la réponse.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755196"
---
# <a name="alternateid"></a><span data-ttu-id="ecc4a-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-103">AlternateId</span></span>

<span data-ttu-id="ecc4a-104">L’élément **AlternateId** décrit un identificateur pour convertir dans une requête et les résultats d’un identificateur converti dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="ecc4a-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecc4a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ecc4a-106">Attributes and elements</span></span>

<span data-ttu-id="ecc4a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecc4a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ecc4a-108">Attributes</span></span>

|<span data-ttu-id="ecc4a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-109">**Attribute**</span></span>|<span data-ttu-id="ecc4a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ecc4a-111">ID</span><span class="sxs-lookup"><span data-stu-id="ecc4a-111">Id</span></span>  <br/> |<span data-ttu-id="ecc4a-112">Décrit l’identificateur source dans une requête [d’opération ConvertId](convertid-operation.md) et l’identificateur de destination dans une réponse de [l’opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ecc4a-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-113">Format</span><span class="sxs-lookup"><span data-stu-id="ecc4a-113">Format</span></span>  <br/> |<span data-ttu-id="ecc4a-114">Décrit le format source dans une requête [d’opération ConvertId](convertid-operation.md) et le format de destination dans une réponse de [l’opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ecc4a-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="ecc4a-115">Le format de destination est décrit par l’attribut **DestinationFormat** de l’élément [ConvertId](convertid.md) dans la demande.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="ecc4a-116">Cet attribut est de type **IdFormatType**.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ecc4a-117">Mailbox</span></span>  <br/> |<span data-ttu-id="ecc4a-118">Décrit l’adresse SMTP Simple Mail Transfer Protocol () principal de la boîte aux lettres qui contient les identificateurs à traduire.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="ecc4a-119">IsArchive</span></span>  <br/> |<span data-ttu-id="ecc4a-120">Indique si l’identificateur représente un élément archivée ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="ecc4a-121">La valeur **true** indique que l’identificateur représente un élément archivée ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="ecc4a-122">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="ecc4a-123">Valeurs d’attribut de format</span><span class="sxs-lookup"><span data-stu-id="ecc4a-123">Format attribute values</span></span>

|<span data-ttu-id="ecc4a-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-124">**Value**</span></span>|<span data-ttu-id="ecc4a-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ecc4a-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="ecc4a-127">Décrit les identificateurs qui sont générées par les Services Web Exchange dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-128">EwsId</span></span>  <br/> |<span data-ttu-id="ecc4a-129">Décrit les identificateurs qui sont générées par les Services Web Exchange commençant par Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-130">Propriété EntryId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-130">EntryId</span></span>  <br/> |<span data-ttu-id="ecc4a-131">Décrit les identificateurs MAPI, comme illustré à la propriété **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="ecc4a-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="ecc4a-133">Décrit une représentation de la propriété **PR_ENTRYID** codé en hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="ecc4a-134">Il s’agit du format des identificateurs d’événement de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-135">StoreId</span></span>  <br/> |<span data-ttu-id="ecc4a-136">Décrit les identificateurs de banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="ecc4a-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-137">OwaId</span></span>  <br/> |<span data-ttu-id="ecc4a-138">Décrit un identificateur d’Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ecc4a-139">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ecc4a-139">Child elements</span></span>

<span data-ttu-id="ecc4a-140">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecc4a-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ecc4a-141">Parent elements</span></span>

|<span data-ttu-id="ecc4a-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-142">**Element**</span></span>|<span data-ttu-id="ecc4a-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="ecc4a-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecc4a-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ecc4a-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="ecc4a-145">Contient l’état et les résultats d’une demande [d’opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ecc4a-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ecc4a-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ecc4a-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="ecc4a-147">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ecc4a-148">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ecc4a-148">Text value</span></span>

<span data-ttu-id="ecc4a-149">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ecc4a-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="ecc4a-150">Remarks</span></span>

<span data-ttu-id="ecc4a-151">L’élément **AlternateId** décrit deux identificateurs, l’identificateur de source doit être convertie dans la requête [d’opération ConvertId](convertid-operation.md) et l’identificateur converti dans l’élément [ConvertIdResponse](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="ecc4a-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="ecc4a-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecc4a-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecc4a-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ecc4a-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="ecc4a-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ecc4a-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ecc4a-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ecc4a-155">Schema Name</span></span>  <br/> |<span data-ttu-id="ecc4a-156">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ecc4a-156">Messages schema</span></span>  <br/> |<span data-ttu-id="ecc4a-157">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ecc4a-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="ecc4a-158">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ecc4a-158">Validation File</span></span>  <br/> |<span data-ttu-id="ecc4a-159">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ecc4a-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="ecc4a-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ecc4a-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ecc4a-161">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ecc4a-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecc4a-162">Faux</span><span class="sxs-lookup"><span data-stu-id="ecc4a-162">False</span></span>  <br/> |<span data-ttu-id="ecc4a-163">Faux</span><span class="sxs-lookup"><span data-stu-id="ecc4a-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecc4a-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ecc4a-164">See also</span></span>

- [<span data-ttu-id="ecc4a-165">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="ecc4a-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="ecc4a-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ecc4a-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ecc4a-167">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="ecc4a-167">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

