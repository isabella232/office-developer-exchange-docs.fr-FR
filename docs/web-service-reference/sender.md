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
description: L’élément de l’expéditeur identifie l’expéditeur d’un élément.
ms.openlocfilehash: a7b06543fadd7cf7ae05f7ae8f86122138e11076
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829323"
---
# <a name="sender"></a><span data-ttu-id="263ca-103">Expéditeur</span><span class="sxs-lookup"><span data-stu-id="263ca-103">Sender</span></span>

<span data-ttu-id="263ca-104">L’élément de **l’expéditeur** identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="263ca-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="263ca-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="263ca-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="263ca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="263ca-106">Attributes and elements</span></span>

<span data-ttu-id="263ca-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="263ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="263ca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="263ca-108">Attributes</span></span>

<span data-ttu-id="263ca-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="263ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="263ca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="263ca-110">Child elements</span></span>

|<span data-ttu-id="263ca-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="263ca-111">**Element**</span></span>|<span data-ttu-id="263ca-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="263ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="263ca-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="263ca-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="263ca-114">Identifie un objet Active Directory de messagerie qui identifie l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="263ca-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="263ca-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="263ca-115">Parent elements</span></span>

|<span data-ttu-id="263ca-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="263ca-116">**Element**</span></span>|<span data-ttu-id="263ca-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="263ca-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="263ca-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="263ca-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="263ca-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-120">Message</span><span class="sxs-lookup"><span data-stu-id="263ca-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="263ca-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="263ca-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="263ca-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="263ca-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="263ca-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="263ca-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="263ca-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="263ca-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="263ca-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="263ca-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="263ca-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="263ca-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="263ca-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="263ca-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="263ca-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="263ca-133">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="263ca-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="263ca-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="263ca-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="263ca-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="263ca-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="263ca-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="263ca-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="263ca-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="263ca-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="263ca-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="263ca-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="263ca-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="263ca-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="263ca-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="263ca-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="263ca-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="263ca-143">Représente l’objet réponse utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="263ca-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="263ca-144">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="263ca-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="263ca-145">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="263ca-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="263ca-146">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="263ca-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="263ca-147">Remarques</span><span class="sxs-lookup"><span data-stu-id="263ca-147">Remarks</span></span>

<span data-ttu-id="263ca-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="263ca-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="263ca-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="263ca-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="263ca-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="263ca-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="263ca-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="263ca-151">Schema Name</span></span>  <br/> |<span data-ttu-id="263ca-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="263ca-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="263ca-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="263ca-153">Validation File</span></span>  <br/> |<span data-ttu-id="263ca-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="263ca-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="263ca-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="263ca-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="263ca-156">False</span><span class="sxs-lookup"><span data-stu-id="263ca-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="263ca-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="263ca-157">See also</span></span>



- [<span data-ttu-id="263ca-158">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="263ca-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

