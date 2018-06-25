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
description: L’élément ConvertId définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755651"
---
# <a name="convertid"></a><span data-ttu-id="a8034-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="a8034-104">ConvertId</span></span>

<span data-ttu-id="a8034-105">L’élément **ConvertId** définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge.</span><span class="sxs-lookup"><span data-stu-id="a8034-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="a8034-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8034-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="a8034-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="a8034-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8034-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8034-108">Attributes and elements</span></span>

<span data-ttu-id="a8034-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8034-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8034-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8034-110">Attributes</span></span>

|<span data-ttu-id="a8034-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a8034-111">**Attribute**</span></span>|<span data-ttu-id="a8034-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8034-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8034-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="a8034-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="a8034-114">Décrit le format d’identificateur qui est renvoyé pour tous les identificateurs convertis.</span><span class="sxs-lookup"><span data-stu-id="a8034-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="a8034-115">Le DestinationFormat est décrit par le IdFormatType.</span><span class="sxs-lookup"><span data-stu-id="a8034-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="a8034-116">Attribut DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="a8034-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="a8034-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a8034-117">**Value**</span></span>|<span data-ttu-id="a8034-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8034-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8034-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="a8034-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="a8034-120">Représente le format d’identificateur qui est utilisé pour les identificateurs de Services Web Exchange qui sont fournis dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="a8034-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="a8034-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="a8034-121">**EwsId**</span></span> <br/> |<span data-ttu-id="a8034-122">Représente le format d’identificateur qui est utilisé pour les identificateurs de Services Web Exchange commençant par Exchange Server 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="a8034-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="a8034-123">**Propriété EntryId**</span><span class="sxs-lookup"><span data-stu-id="a8034-123">**EntryId**</span></span> <br/> |<span data-ttu-id="a8034-124">Représente l’identificateur MAPI, comme illustré à la propriété PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="a8034-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="a8034-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="a8034-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="a8034-126">Représente l’identificateur d’événement disponibilité calendrier.</span><span class="sxs-lookup"><span data-stu-id="a8034-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="a8034-127">Il s’agit d’une représentation de la propriété PR_ENTRYID codé en hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="a8034-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="a8034-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="a8034-128">**StoreId**</span></span> <br/> |<span data-ttu-id="a8034-129">Représente l’identificateur de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8034-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="a8034-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="a8034-130">**OwaId**</span></span> <br/> |<span data-ttu-id="a8034-131">Représente le format d’identificateur d’Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="a8034-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a8034-132">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8034-132">Child elements</span></span>

|<span data-ttu-id="a8034-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8034-133">**Element**</span></span>|<span data-ttu-id="a8034-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8034-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8034-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="a8034-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="a8034-136">Contient les identificateurs source à convertir.</span><span class="sxs-lookup"><span data-stu-id="a8034-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8034-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8034-137">Parent elements</span></span>

<span data-ttu-id="a8034-138">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8034-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8034-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8034-139">Remarks</span></span>

<span data-ttu-id="a8034-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a8034-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8034-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8034-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8034-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8034-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8034-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8034-143">Schema Name</span></span>  <br/> |<span data-ttu-id="a8034-144">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="a8034-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="a8034-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8034-145">Validation File</span></span>  <br/> |<span data-ttu-id="a8034-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8034-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8034-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8034-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8034-148">False</span><span class="sxs-lookup"><span data-stu-id="a8034-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8034-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8034-149">See also</span></span>



[<span data-ttu-id="a8034-150">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="a8034-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="a8034-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8034-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a8034-152">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="a8034-152">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

