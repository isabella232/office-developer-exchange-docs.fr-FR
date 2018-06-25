---
title: GetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: L’élément GetHoldOnMailboxesResponseMessage Spécifie le message de réponse pour une demande GetHoldOnMailboxes.
ms.openlocfilehash: e1c43f75bfa62b20de9248546e71c92ae5998ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756634"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="2ceed-103">GetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2ceed-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="2ceed-104">L’élément **GetHoldOnMailboxesResponseMessage** Spécifie le message de réponse pour une demande **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="2ceed-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="2ceed-105">**GetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2ceed-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ceed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ceed-106">Attributes and elements</span></span>

<span data-ttu-id="2ceed-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ceed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ceed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ceed-108">Attributes</span></span>

|<span data-ttu-id="2ceed-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2ceed-109">**Attribute**</span></span>|<span data-ttu-id="2ceed-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ceed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ceed-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="2ceed-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="2ceed-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="2ceed-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="2ceed-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="2ceed-113">ResponseClass</span></span>

|<span data-ttu-id="2ceed-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2ceed-114">**Value**</span></span>|<span data-ttu-id="2ceed-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ceed-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ceed-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="2ceed-116">Success</span></span>  <br/> |<span data-ttu-id="2ceed-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="2ceed-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="2ceed-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="2ceed-118">Warning</span></span>  <br/> |<span data-ttu-id="2ceed-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="2ceed-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="2ceed-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="2ceed-120">Error</span></span>  <br/> |<span data-ttu-id="2ceed-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="2ceed-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2ceed-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ceed-122">Child elements</span></span>

|<span data-ttu-id="2ceed-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ceed-123">**Element**</span></span>|<span data-ttu-id="2ceed-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ceed-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ceed-125">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="2ceed-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="2ceed-126">Contient le résultat de la demande **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="2ceed-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="2ceed-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2ceed-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2ceed-128">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="2ceed-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="2ceed-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="2ceed-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2ceed-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="2ceed-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2ceed-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2ceed-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2ceed-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="2ceed-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2ceed-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2ceed-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2ceed-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="2ceed-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ceed-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ceed-135">Parent elements</span></span>

|<span data-ttu-id="2ceed-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ceed-136">**Element**</span></span>|<span data-ttu-id="2ceed-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ceed-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ceed-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2ceed-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2ceed-139">Contient les messages de réponse pour une demande d’Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="2ceed-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2ceed-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ceed-140">Remarks</span></span>

<span data-ttu-id="2ceed-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2ceed-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ceed-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ceed-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ceed-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ceed-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ceed-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ceed-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ceed-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ceed-145">Schema Name</span></span>  <br/> |<span data-ttu-id="2ceed-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="2ceed-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="2ceed-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ceed-147">Validation File</span></span>  <br/> |<span data-ttu-id="2ceed-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2ceed-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ceed-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ceed-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2ceed-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ceed-150">See also</span></span>



- [<span data-ttu-id="2ceed-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ceed-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

