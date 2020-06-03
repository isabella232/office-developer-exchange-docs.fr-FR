---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: L’élément GetConversationItemsResponseMessage spécifie le message de réponse pour une demande GetConversationItems.
ms.openlocfilehash: b38bca60bb51c24a7635391c4e23e5426366cd72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461071"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="d3f53-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3f53-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="d3f53-104">L’élément **GetConversationItemsResponseMessage** spécifie le message de réponse pour une demande **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="d3f53-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="d3f53-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d3f53-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3f53-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3f53-106">Attributes and elements</span></span>

<span data-ttu-id="d3f53-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3f53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3f53-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3f53-108">Attributes</span></span>

|<span data-ttu-id="d3f53-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d3f53-109">**Attribute**</span></span>|<span data-ttu-id="d3f53-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3f53-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3f53-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d3f53-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="d3f53-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d3f53-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="d3f53-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d3f53-113">ResponseClass</span></span>

|<span data-ttu-id="d3f53-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d3f53-114">**Value**</span></span>|<span data-ttu-id="d3f53-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3f53-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3f53-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="d3f53-116">Success</span></span>  <br/> |<span data-ttu-id="d3f53-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="d3f53-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="d3f53-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="d3f53-118">Warning</span></span>  <br/> |<span data-ttu-id="d3f53-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="d3f53-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="d3f53-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="d3f53-120">Error</span></span>  <br/> |<span data-ttu-id="d3f53-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="d3f53-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d3f53-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3f53-122">Child elements</span></span>

|<span data-ttu-id="d3f53-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3f53-123">**Element**</span></span>|<span data-ttu-id="d3f53-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3f53-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3f53-125">Conversation (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="d3f53-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="d3f53-126">Représente une conversation unique renvoyée dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="d3f53-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="d3f53-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d3f53-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d3f53-128">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d3f53-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="d3f53-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="d3f53-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d3f53-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d3f53-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d3f53-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d3f53-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d3f53-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="d3f53-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d3f53-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3f53-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d3f53-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="d3f53-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3f53-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3f53-135">Parent elements</span></span>

|<span data-ttu-id="d3f53-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3f53-136">**Element**</span></span>|<span data-ttu-id="d3f53-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3f53-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3f53-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3f53-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d3f53-139">Contient les messages de réponse pour une demande de services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d3f53-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3f53-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3f53-140">Remarks</span></span>

<span data-ttu-id="d3f53-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d3f53-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d3f53-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3f53-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3f53-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3f53-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3f53-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3f53-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3f53-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3f53-145">Schema Name</span></span>  <br/> |<span data-ttu-id="d3f53-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="d3f53-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="d3f53-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3f53-147">Validation File</span></span>  <br/> |<span data-ttu-id="d3f53-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d3f53-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3f53-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3f53-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d3f53-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3f53-150">See also</span></span>



- [<span data-ttu-id="d3f53-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d3f53-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

