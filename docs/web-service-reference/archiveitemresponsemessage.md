---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: L’élément ArchiveItemResponseMessage spécifie le message de réponse à une demande ArchiveItem.
ms.openlocfilehash: 24d09d63cab6805194e35031d8590290573de0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463390"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="29d38-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29d38-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="29d38-104">L’élément **ArchiveItemResponseMessage** spécifie le message de réponse à une demande **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="29d38-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="29d38-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="29d38-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29d38-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="29d38-106">Attributes and elements</span></span>

<span data-ttu-id="29d38-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="29d38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29d38-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="29d38-108">Attributes</span></span>

|<span data-ttu-id="29d38-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="29d38-109">**Attribute**</span></span>|<span data-ttu-id="29d38-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="29d38-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29d38-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="29d38-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="29d38-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="29d38-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="29d38-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="29d38-113">ResponseClass</span></span>

|<span data-ttu-id="29d38-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="29d38-114">**Value**</span></span>|<span data-ttu-id="29d38-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="29d38-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29d38-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="29d38-116">Success</span></span>  <br/> |<span data-ttu-id="29d38-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="29d38-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="29d38-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="29d38-118">Warning</span></span>  <br/> |<span data-ttu-id="29d38-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="29d38-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="29d38-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="29d38-120">Error</span></span>  <br/> |<span data-ttu-id="29d38-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="29d38-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="29d38-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="29d38-122">Child elements</span></span>

|<span data-ttu-id="29d38-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29d38-123">**Element**</span></span>|<span data-ttu-id="29d38-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="29d38-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29d38-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="29d38-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="29d38-126">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="29d38-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="29d38-127">Items</span><span class="sxs-lookup"><span data-stu-id="29d38-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="29d38-128">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="29d38-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="29d38-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="29d38-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="29d38-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="29d38-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="29d38-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="29d38-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="29d38-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="29d38-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="29d38-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29d38-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="29d38-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="29d38-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29d38-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="29d38-135">Parent elements</span></span>

|<span data-ttu-id="29d38-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29d38-136">**Element**</span></span>|<span data-ttu-id="29d38-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="29d38-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29d38-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29d38-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="29d38-139">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="29d38-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29d38-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="29d38-140">Remarks</span></span>

<span data-ttu-id="29d38-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="29d38-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="29d38-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="29d38-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29d38-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="29d38-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29d38-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="29d38-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29d38-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="29d38-145">Schema Name</span></span>  <br/> |<span data-ttu-id="29d38-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="29d38-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="29d38-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="29d38-147">Validation File</span></span>  <br/> |<span data-ttu-id="29d38-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="29d38-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29d38-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="29d38-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="29d38-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29d38-150">See also</span></span>

- [<span data-ttu-id="29d38-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29d38-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

