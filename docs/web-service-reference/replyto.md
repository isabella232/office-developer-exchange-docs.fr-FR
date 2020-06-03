---
title: ReplyTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyTo
api_type:
- schema
ms.assetid: 6b6ae792-e2c4-4aa0-95cb-b49b446f1e08
description: L’élément ReplyTo identifie un tableau d’adresses auxquelles les réponses doivent être envoyées.
ms.openlocfilehash: 08f9edce76fd01111922a2a07d1a63e288a0c1ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468326"
---
# <a name="replyto"></a><span data-ttu-id="be743-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="be743-103">ReplyTo</span></span>

<span data-ttu-id="be743-104">L’élément **ReplyTo** identifie un tableau d’adresses auxquelles les réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="be743-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="be743-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="be743-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be743-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="be743-106">Attributes and elements</span></span>

<span data-ttu-id="be743-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="be743-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be743-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="be743-108">Attributes</span></span>

<span data-ttu-id="be743-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="be743-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be743-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="be743-110">Child elements</span></span>

|<span data-ttu-id="be743-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be743-111">**Element**</span></span>|<span data-ttu-id="be743-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="be743-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be743-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="be743-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="be743-114">Identifie un objet de service d’annuaire Active Directory à extension messagerie auquel une réponse est envoyée.</span><span class="sxs-lookup"><span data-stu-id="be743-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be743-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="be743-115">Parent elements</span></span>

|<span data-ttu-id="be743-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be743-116">**Element**</span></span>|<span data-ttu-id="be743-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="be743-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be743-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="be743-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="be743-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-120">Message</span><span class="sxs-lookup"><span data-stu-id="be743-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="be743-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="be743-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="be743-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="be743-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-124">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="be743-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="be743-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="be743-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="be743-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="be743-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="be743-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="be743-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="be743-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="be743-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="be743-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="be743-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="be743-133">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="be743-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="be743-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="be743-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="be743-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="be743-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="be743-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="be743-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="be743-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="be743-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="be743-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be743-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be743-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="be743-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="be743-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="be743-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="be743-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="be743-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="be743-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="be743-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="be743-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="be743-144">Remarks</span></span>

<span data-ttu-id="be743-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="be743-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be743-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="be743-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be743-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="be743-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be743-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="be743-148">Schema Name</span></span>  <br/> |<span data-ttu-id="be743-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="be743-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="be743-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="be743-150">Validation File</span></span>  <br/> |<span data-ttu-id="be743-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="be743-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be743-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="be743-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="be743-153">False</span><span class="sxs-lookup"><span data-stu-id="be743-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be743-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be743-154">See also</span></span>



- [<span data-ttu-id="be743-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="be743-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

