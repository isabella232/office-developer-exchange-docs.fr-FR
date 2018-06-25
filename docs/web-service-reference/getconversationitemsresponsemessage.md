---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: L’élément GetConversationItemsResponseMessage Spécifie le message de réponse pour une demande GetConversationItems.
ms.openlocfilehash: 997319193311ef9267d8f6ff14c70bfe40e2634b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756559"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="9f128-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f128-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="9f128-104">L’élément **GetConversationItemsResponseMessage** Spécifie le message de réponse pour une demande **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="9f128-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="9f128-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9f128-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f128-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f128-106">Attributes and elements</span></span>

<span data-ttu-id="9f128-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f128-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f128-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f128-108">Attributes</span></span>

|<span data-ttu-id="9f128-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9f128-109">**Attribute**</span></span>|<span data-ttu-id="9f128-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f128-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f128-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9f128-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="9f128-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="9f128-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="9f128-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9f128-113">ResponseClass</span></span>

|<span data-ttu-id="9f128-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9f128-114">**Value**</span></span>|<span data-ttu-id="9f128-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f128-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f128-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="9f128-116">Success</span></span>  <br/> |<span data-ttu-id="9f128-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="9f128-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="9f128-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="9f128-118">Warning</span></span>  <br/> |<span data-ttu-id="9f128-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="9f128-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="9f128-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="9f128-120">Error</span></span>  <br/> |<span data-ttu-id="9f128-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="9f128-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f128-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f128-122">Child elements</span></span>

|<span data-ttu-id="9f128-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f128-123">**Element**</span></span>|<span data-ttu-id="9f128-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f128-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f128-125">Conversation (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="9f128-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="9f128-126">Représente une seule conversation renvoyée dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="9f128-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="9f128-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9f128-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9f128-128">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="9f128-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="9f128-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="9f128-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9f128-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="9f128-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9f128-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9f128-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9f128-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="9f128-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9f128-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9f128-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9f128-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="9f128-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f128-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f128-135">Parent elements</span></span>

|<span data-ttu-id="9f128-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f128-136">**Element**</span></span>|<span data-ttu-id="9f128-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f128-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f128-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f128-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f128-139">Contient les messages de réponse pour une demande d’Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="9f128-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f128-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f128-140">Remarks</span></span>

<span data-ttu-id="9f128-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f128-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f128-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f128-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f128-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f128-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f128-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f128-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f128-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f128-145">Schema Name</span></span>  <br/> |<span data-ttu-id="9f128-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="9f128-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="9f128-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f128-147">Validation File</span></span>  <br/> |<span data-ttu-id="9f128-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f128-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f128-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f128-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9f128-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f128-150">See also</span></span>



- [<span data-ttu-id="9f128-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f128-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

