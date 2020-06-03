---
title: Expéditeur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda
description: L’élément sender identifie l’expéditeur d’un élément.
ms.openlocfilehash: f056fefdd5c5832d4b5bf20416e07e376f6a03de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530578"
---
# <a name="sender"></a><span data-ttu-id="1e2f0-103">Expéditeur</span><span class="sxs-lookup"><span data-stu-id="1e2f0-103">Sender</span></span>

<span data-ttu-id="1e2f0-104">L’élément **sender** identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="1e2f0-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="1e2f0-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e2f0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e2f0-106">Attributes and elements</span></span>

<span data-ttu-id="1e2f0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e2f0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e2f0-108">Attributes</span></span>

<span data-ttu-id="1e2f0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e2f0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e2f0-110">Child elements</span></span>

|<span data-ttu-id="1e2f0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e2f0-111">**Element**</span></span>|<span data-ttu-id="1e2f0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e2f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e2f0-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="1e2f0-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="1e2f0-114">Identifie un objet Active Directory à extension messagerie qui identifie l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e2f0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e2f0-115">Parent elements</span></span>

|<span data-ttu-id="1e2f0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e2f0-116">**Element**</span></span>|<span data-ttu-id="1e2f0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e2f0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e2f0-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="1e2f0-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-120">Message</span><span class="sxs-lookup"><span data-stu-id="1e2f0-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1e2f0-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="1e2f0-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="1e2f0-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-124">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="1e2f0-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1e2f0-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1e2f0-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="1e2f0-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="1e2f0-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="1e2f0-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="1e2f0-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="1e2f0-133">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="1e2f0-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="1e2f0-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="1e2f0-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="1e2f0-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="1e2f0-143">Représente l’objet de réponse utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="1e2f0-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="1e2f0-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="1e2f0-145">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="1e2f0-146">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1e2f0-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1e2f0-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e2f0-147">Remarks</span></span>

<span data-ttu-id="1e2f0-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1e2f0-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e2f0-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e2f0-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e2f0-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e2f0-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e2f0-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e2f0-151">Schema Name</span></span>  <br/> |<span data-ttu-id="1e2f0-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1e2f0-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e2f0-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e2f0-153">Validation File</span></span>  <br/> |<span data-ttu-id="1e2f0-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e2f0-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e2f0-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e2f0-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e2f0-156">False</span><span class="sxs-lookup"><span data-stu-id="1e2f0-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e2f0-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e2f0-157">See also</span></span>



- [<span data-ttu-id="1e2f0-158">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e2f0-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

