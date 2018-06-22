---
title: De
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: L’élément de représente l’adresse à partir de laquelle le message a été envoyé.
ms.openlocfilehash: 39c8c8ef84ff445e8f44ebb9f2285ccfc42353a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756496"
---
# <a name="from"></a><span data-ttu-id="e51c9-103">De</span><span class="sxs-lookup"><span data-stu-id="e51c9-103">From</span></span>

<span data-ttu-id="e51c9-104">L’élément **à partir de** représente l’adresse à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="e51c9-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="e51c9-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="e51c9-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e51c9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e51c9-106">Attributes and elements</span></span>

<span data-ttu-id="e51c9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e51c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e51c9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e51c9-108">Attributes</span></span>

<span data-ttu-id="e51c9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e51c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e51c9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e51c9-110">Child elements</span></span>

|<span data-ttu-id="e51c9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e51c9-111">**Element**</span></span>|<span data-ttu-id="e51c9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e51c9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e51c9-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="e51c9-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e51c9-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e51c9-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e51c9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e51c9-115">Parent elements</span></span>

|<span data-ttu-id="e51c9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e51c9-116">**Element**</span></span>|<span data-ttu-id="e51c9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e51c9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e51c9-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e51c9-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-120">Message</span><span class="sxs-lookup"><span data-stu-id="e51c9-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e51c9-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e51c9-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e51c9-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e51c9-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e51c9-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e51c9-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e51c9-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e51c9-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e51c9-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="e51c9-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="e51c9-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="e51c9-133">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="e51c9-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="e51c9-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="e51c9-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="e51c9-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="e51c9-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="e51c9-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="e51c9-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="e51c9-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="e51c9-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e51c9-144">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="e51c9-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="e51c9-145">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e51c9-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="e51c9-146">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e51c9-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e51c9-147">Note</span><span class="sxs-lookup"><span data-stu-id="e51c9-147">Remarks</span></span>

<span data-ttu-id="e51c9-148">Cet élément est utilisé pour « envoyer de la part de » des messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="e51c9-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="e51c9-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e51c9-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e51c9-150">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e51c9-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e51c9-151">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e51c9-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e51c9-152">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e51c9-152">Schema Name</span></span>  <br/> |<span data-ttu-id="e51c9-153">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e51c9-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="e51c9-154">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e51c9-154">Validation File</span></span>  <br/> |<span data-ttu-id="e51c9-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e51c9-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e51c9-156">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e51c9-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="e51c9-157">False</span><span class="sxs-lookup"><span data-stu-id="e51c9-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e51c9-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e51c9-158">See also</span></span>



- [<span data-ttu-id="e51c9-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e51c9-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

