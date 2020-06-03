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
description: L’élément AlternateId décrit un identificateur à convertir dans une requête et les résultats d’un identificateur converti dans la réponse.
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527452"
---
# <a name="alternateid"></a><span data-ttu-id="955d5-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="955d5-103">AlternateId</span></span>

<span data-ttu-id="955d5-104">L’élément **AlternateId** décrit un identificateur à convertir dans une requête et les résultats d’un identificateur converti dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="955d5-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="955d5-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="955d5-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="955d5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="955d5-106">Attributes and elements</span></span>

<span data-ttu-id="955d5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="955d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="955d5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="955d5-108">Attributes</span></span>

|<span data-ttu-id="955d5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="955d5-109">**Attribute**</span></span>|<span data-ttu-id="955d5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="955d5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="955d5-111">ID</span><span class="sxs-lookup"><span data-stu-id="955d5-111">Id</span></span>  <br/> |<span data-ttu-id="955d5-112">Décrit l’identificateur source dans une demande d' [opération ConvertId](convertid-operation.md) et décrit l’identificateur de destination dans une réponse d' [opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="955d5-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="955d5-113">Format</span><span class="sxs-lookup"><span data-stu-id="955d5-113">Format</span></span>  <br/> |<span data-ttu-id="955d5-114">Décrit le format source dans une demande d' [opération ConvertId](convertid-operation.md) et décrit le format de destination dans une réponse de l' [opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="955d5-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="955d5-115">Le format de destination est décrit par l’attribut **DestinationFormat** de l’élément [ConvertId](convertid.md) dans la demande.</span><span class="sxs-lookup"><span data-stu-id="955d5-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="955d5-116">Cet attribut est de type **IdFormatType**.</span><span class="sxs-lookup"><span data-stu-id="955d5-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="955d5-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="955d5-117">Mailbox</span></span>  <br/> |<span data-ttu-id="955d5-118">Décrit l’adresse SMTP (Simple Mail Transfer Protocol) principale de la boîte aux lettres qui contient les identificateurs à traduire.</span><span class="sxs-lookup"><span data-stu-id="955d5-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="955d5-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="955d5-119">IsArchive</span></span>  <br/> |<span data-ttu-id="955d5-120">Indique si l’identificateur représente un élément ou un dossier archivé.</span><span class="sxs-lookup"><span data-stu-id="955d5-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="955d5-121">La valeur **true** indique que l’identificateur représente un élément ou un dossier archivé.</span><span class="sxs-lookup"><span data-stu-id="955d5-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="955d5-122">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="955d5-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="955d5-123">Valeurs de l’attribut format</span><span class="sxs-lookup"><span data-stu-id="955d5-123">Format attribute values</span></span>

|<span data-ttu-id="955d5-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="955d5-124">**Value**</span></span>|<span data-ttu-id="955d5-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="955d5-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="955d5-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="955d5-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="955d5-127">Décrit les identificateurs générés par les services Web Exchange dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="955d5-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="955d5-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="955d5-128">EwsId</span></span>  <br/> |<span data-ttu-id="955d5-129">Décrit les identificateurs générés par les services Web Exchange à partir d’Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="955d5-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="955d5-130">Entrée</span><span class="sxs-lookup"><span data-stu-id="955d5-130">EntryId</span></span>  <br/> |<span data-ttu-id="955d5-131">Décrit les identificateurs MAPI, comme dans la propriété **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="955d5-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="955d5-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="955d5-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="955d5-133">Décrit une représentation codée en hexadécimal de la propriété **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="955d5-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="955d5-134">Il s’agit du format des identificateurs d’événements de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="955d5-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="955d5-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="955d5-135">StoreId</span></span>  <br/> |<span data-ttu-id="955d5-136">Décrit les identificateurs de banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="955d5-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="955d5-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="955d5-137">OwaId</span></span>  <br/> |<span data-ttu-id="955d5-138">Décrit un identificateur Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="955d5-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="955d5-139">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="955d5-139">Child elements</span></span>

<span data-ttu-id="955d5-140">Aucun.</span><span class="sxs-lookup"><span data-stu-id="955d5-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="955d5-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="955d5-141">Parent elements</span></span>

|<span data-ttu-id="955d5-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="955d5-142">**Element**</span></span>|<span data-ttu-id="955d5-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="955d5-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="955d5-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="955d5-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="955d5-145">Contient l’État et le résultat d’une demande d' [opération ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="955d5-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="955d5-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="955d5-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="955d5-147">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="955d5-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="955d5-148">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="955d5-148">Text value</span></span>

<span data-ttu-id="955d5-149">Aucun.</span><span class="sxs-lookup"><span data-stu-id="955d5-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="955d5-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="955d5-150">Remarks</span></span>

<span data-ttu-id="955d5-151">L’élément **AlternateId** décrit deux identificateurs, l’identificateur source à convertir dans la demande d' [opération ConvertId](convertid-operation.md) et l’identificateur converti dans l’élément [ConvertIdResponse](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="955d5-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="955d5-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="955d5-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="955d5-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="955d5-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="955d5-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="955d5-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="955d5-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="955d5-155">Schema Name</span></span>  <br/> |<span data-ttu-id="955d5-156">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="955d5-156">Messages schema</span></span>  <br/> |<span data-ttu-id="955d5-157">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="955d5-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="955d5-158">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="955d5-158">Validation File</span></span>  <br/> |<span data-ttu-id="955d5-159">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="955d5-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="955d5-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="955d5-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="955d5-161">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="955d5-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="955d5-162">False</span><span class="sxs-lookup"><span data-stu-id="955d5-162">False</span></span>  <br/> |<span data-ttu-id="955d5-163">False</span><span class="sxs-lookup"><span data-stu-id="955d5-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="955d5-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="955d5-164">See also</span></span>

- [<span data-ttu-id="955d5-165">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="955d5-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="955d5-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="955d5-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="955d5-167">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="955d5-167">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

