---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: L’élément ConvertId définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452537"
---
# <a name="convertid"></a><span data-ttu-id="aae22-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="aae22-104">ConvertId</span></span>

<span data-ttu-id="aae22-105">L’élément **ConvertId** définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge.</span><span class="sxs-lookup"><span data-stu-id="aae22-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="aae22-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="aae22-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="aae22-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="aae22-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aae22-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aae22-108">Attributes and elements</span></span>

<span data-ttu-id="aae22-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aae22-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aae22-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="aae22-110">Attributes</span></span>

|<span data-ttu-id="aae22-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="aae22-111">**Attribute**</span></span>|<span data-ttu-id="aae22-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aae22-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aae22-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="aae22-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="aae22-114">Décrit le format d’identificateur qui sera renvoyé pour tous les identificateurs convertis.</span><span class="sxs-lookup"><span data-stu-id="aae22-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="aae22-115">Le DestinationFormat est décrit par le IdFormatType.</span><span class="sxs-lookup"><span data-stu-id="aae22-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="aae22-116">Attribut DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="aae22-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="aae22-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="aae22-117">**Value**</span></span>|<span data-ttu-id="aae22-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="aae22-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aae22-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="aae22-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="aae22-120">Représente le format d’identificateur utilisé pour les identificateurs de services Web Exchange fournis dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="aae22-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="aae22-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="aae22-121">**EwsId**</span></span> <br/> |<span data-ttu-id="aae22-122">Représente le format d’identificateur utilisé pour les identificateurs de services Web Exchange à partir d’Exchange Server 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="aae22-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="aae22-123">**Entrée**</span><span class="sxs-lookup"><span data-stu-id="aae22-123">**EntryId**</span></span> <br/> |<span data-ttu-id="aae22-124">Représente l’identificateur MAPI, comme dans la propriété PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="aae22-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="aae22-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="aae22-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="aae22-126">Représente l’identificateur d’événement de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="aae22-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="aae22-127">Il s’agit d’une représentation codée en hexadécimal de la propriété PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="aae22-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="aae22-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="aae22-128">**StoreId**</span></span> <br/> |<span data-ttu-id="aae22-129">Représente l’identificateur de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="aae22-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="aae22-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="aae22-130">**OwaId**</span></span> <br/> |<span data-ttu-id="aae22-131">Représente le format d’identificateur d’Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="aae22-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aae22-132">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aae22-132">Child elements</span></span>

|<span data-ttu-id="aae22-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aae22-133">**Element**</span></span>|<span data-ttu-id="aae22-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="aae22-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aae22-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="aae22-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="aae22-136">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="aae22-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aae22-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aae22-137">Parent elements</span></span>

<span data-ttu-id="aae22-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aae22-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aae22-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="aae22-139">Remarks</span></span>

<span data-ttu-id="aae22-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="aae22-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aae22-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aae22-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aae22-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aae22-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aae22-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aae22-143">Schema Name</span></span>  <br/> |<span data-ttu-id="aae22-144">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="aae22-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="aae22-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aae22-145">Validation File</span></span>  <br/> |<span data-ttu-id="aae22-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aae22-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aae22-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aae22-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="aae22-148">False</span><span class="sxs-lookup"><span data-stu-id="aae22-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aae22-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aae22-149">See also</span></span>



[<span data-ttu-id="aae22-150">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="aae22-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="aae22-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aae22-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="aae22-152">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="aae22-152">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

