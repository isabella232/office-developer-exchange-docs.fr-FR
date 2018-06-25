---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: L’élément GetSearchableMailboxesResponseMessage Spécifie le message de réponse pour une demande GetSearchableMailboxes.
ms.openlocfilehash: 2a4d1fe357656fe29d8572e7f32a4bc2e4a6131e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756742"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="3efe1-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3efe1-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="3efe1-104">L’élément **GetSearchableMailboxesResponseMessage** Spécifie le message de réponse pour une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="3efe1-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="3efe1-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3efe1-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3efe1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3efe1-106">Attributes and elements</span></span>

<span data-ttu-id="3efe1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3efe1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3efe1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3efe1-108">Attributes</span></span>

|<span data-ttu-id="3efe1-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3efe1-109">**Attribute**</span></span>|<span data-ttu-id="3efe1-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="3efe1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3efe1-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3efe1-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="3efe1-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="3efe1-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="3efe1-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3efe1-113">ResponseClass</span></span>

|<span data-ttu-id="3efe1-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="3efe1-114">**Value**</span></span>|<span data-ttu-id="3efe1-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="3efe1-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3efe1-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="3efe1-116">Success</span></span>  <br/> |<span data-ttu-id="3efe1-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="3efe1-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="3efe1-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="3efe1-118">Warning</span></span>  <br/> |<span data-ttu-id="3efe1-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="3efe1-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="3efe1-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="3efe1-120">Error</span></span>  <br/> |<span data-ttu-id="3efe1-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="3efe1-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3efe1-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3efe1-122">Child elements</span></span>

|<span data-ttu-id="3efe1-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3efe1-123">**Element**</span></span>|<span data-ttu-id="3efe1-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="3efe1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3efe1-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="3efe1-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="3efe1-126">Contient un tableau de boîtes aux lettres renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="3efe1-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="3efe1-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3efe1-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3efe1-128">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="3efe1-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="3efe1-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="3efe1-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3efe1-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="3efe1-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3efe1-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3efe1-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3efe1-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="3efe1-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3efe1-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3efe1-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3efe1-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="3efe1-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3efe1-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3efe1-135">Parent elements</span></span>

|<span data-ttu-id="3efe1-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3efe1-136">**Element**</span></span>|<span data-ttu-id="3efe1-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="3efe1-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3efe1-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3efe1-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3efe1-139">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3efe1-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3efe1-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="3efe1-140">Remarks</span></span>

<span data-ttu-id="3efe1-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3efe1-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3efe1-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3efe1-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3efe1-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3efe1-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3efe1-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3efe1-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3efe1-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3efe1-145">Schema Name</span></span>  <br/> |<span data-ttu-id="3efe1-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="3efe1-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="3efe1-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3efe1-147">Validation File</span></span>  <br/> |<span data-ttu-id="3efe1-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3efe1-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3efe1-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3efe1-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3efe1-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3efe1-150">See also</span></span>



- [<span data-ttu-id="3efe1-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3efe1-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

