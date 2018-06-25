---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: L’élément ArchiveItemResponseMessage Spécifie le message de réponse à une demande de ArchiveItem.
ms.openlocfilehash: a7832e2cb4ec91a0871de5979fd1b418c0626aa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755318"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="7ed13-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ed13-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="7ed13-104">L’élément **ArchiveItemResponseMessage** Spécifie le message de réponse à une demande de **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="7ed13-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="7ed13-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7ed13-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ed13-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7ed13-106">Attributes and elements</span></span>

<span data-ttu-id="7ed13-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7ed13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ed13-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7ed13-108">Attributes</span></span>

|<span data-ttu-id="7ed13-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7ed13-109">**Attribute**</span></span>|<span data-ttu-id="7ed13-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ed13-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ed13-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7ed13-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="7ed13-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7ed13-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="7ed13-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7ed13-113">ResponseClass</span></span>

|<span data-ttu-id="7ed13-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7ed13-114">**Value**</span></span>|<span data-ttu-id="7ed13-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ed13-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ed13-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="7ed13-116">Success</span></span>  <br/> |<span data-ttu-id="7ed13-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="7ed13-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="7ed13-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="7ed13-118">Warning</span></span>  <br/> |<span data-ttu-id="7ed13-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="7ed13-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="7ed13-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="7ed13-120">Error</span></span>  <br/> |<span data-ttu-id="7ed13-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="7ed13-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7ed13-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7ed13-122">Child elements</span></span>

|<span data-ttu-id="7ed13-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ed13-123">**Element**</span></span>|<span data-ttu-id="7ed13-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ed13-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ed13-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7ed13-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7ed13-126">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="7ed13-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="7ed13-127">Items</span><span class="sxs-lookup"><span data-stu-id="7ed13-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="7ed13-128">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="7ed13-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="7ed13-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="7ed13-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7ed13-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7ed13-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7ed13-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7ed13-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7ed13-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="7ed13-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7ed13-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ed13-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7ed13-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="7ed13-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ed13-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7ed13-135">Parent elements</span></span>

|<span data-ttu-id="7ed13-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7ed13-136">**Element**</span></span>|<span data-ttu-id="7ed13-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="7ed13-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ed13-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7ed13-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7ed13-139">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ed13-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ed13-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="7ed13-140">Remarks</span></span>

<span data-ttu-id="7ed13-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7ed13-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7ed13-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ed13-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ed13-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7ed13-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ed13-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7ed13-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7ed13-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7ed13-145">Schema Name</span></span>  <br/> |<span data-ttu-id="7ed13-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="7ed13-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="7ed13-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7ed13-147">Validation File</span></span>  <br/> |<span data-ttu-id="7ed13-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7ed13-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7ed13-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7ed13-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7ed13-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ed13-150">See also</span></span>

- [<span data-ttu-id="7ed13-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7ed13-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

