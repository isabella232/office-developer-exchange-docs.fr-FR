---
title: From
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
description: L’élément from représente l’adresse à partir de laquelle le message a été envoyé.
ms.openlocfilehash: c0d655731677e56cc02c7c029264ffc96f0a18c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459552"
---
# <a name="from"></a><span data-ttu-id="2d0cb-103">From</span><span class="sxs-lookup"><span data-stu-id="2d0cb-103">From</span></span>

<span data-ttu-id="2d0cb-104">L’élément **from** représente l’adresse à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="2d0cb-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="2d0cb-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d0cb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d0cb-106">Attributes and elements</span></span>

<span data-ttu-id="2d0cb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d0cb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d0cb-108">Attributes</span></span>

<span data-ttu-id="2d0cb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d0cb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d0cb-110">Child elements</span></span>

|<span data-ttu-id="2d0cb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d0cb-111">**Element**</span></span>|<span data-ttu-id="2d0cb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d0cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d0cb-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="2d0cb-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="2d0cb-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d0cb-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d0cb-115">Parent elements</span></span>

|<span data-ttu-id="2d0cb-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d0cb-116">**Element**</span></span>|<span data-ttu-id="2d0cb-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d0cb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d0cb-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2d0cb-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-120">Message</span><span class="sxs-lookup"><span data-stu-id="2d0cb-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2d0cb-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2d0cb-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2d0cb-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-124">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2d0cb-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2d0cb-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2d0cb-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2d0cb-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2d0cb-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2d0cb-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="2d0cb-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="2d0cb-133">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="2d0cb-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="2d0cb-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="2d0cb-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="2d0cb-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="2d0cb-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="2d0cb-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="2d0cb-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2d0cb-145">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="2d0cb-146">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2d0cb-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d0cb-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d0cb-147">Remarks</span></span>

<span data-ttu-id="2d0cb-148">Cet élément est utilisé pour les messages électroniques « envoyer de la part de ».</span><span class="sxs-lookup"><span data-stu-id="2d0cb-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="2d0cb-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2d0cb-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d0cb-150">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d0cb-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d0cb-151">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d0cb-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d0cb-152">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d0cb-152">Schema Name</span></span>  <br/> |<span data-ttu-id="2d0cb-153">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2d0cb-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d0cb-154">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d0cb-154">Validation File</span></span>  <br/> |<span data-ttu-id="2d0cb-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d0cb-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d0cb-156">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d0cb-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d0cb-157">False</span><span class="sxs-lookup"><span data-stu-id="2d0cb-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d0cb-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d0cb-158">See also</span></span>



- [<span data-ttu-id="2d0cb-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2d0cb-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

