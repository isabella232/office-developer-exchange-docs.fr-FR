---
title: ReceivedBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedBy
api_type:
- schema
ms.assetid: ac84c9c5-d2fe-4b6f-bf4d-0444131d835b
description: L’élément ReceivedBy identifie le délégué dans un scénario d’accès délégué.
ms.openlocfilehash: 7cee996c15e81f77d71f42e052b14b1d21772ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468249"
---
# <a name="receivedby"></a><span data-ttu-id="f6000-103">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="f6000-103">ReceivedBy</span></span>

<span data-ttu-id="f6000-104">L’élément **ReceivedBy** identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="f6000-104">The **ReceivedBy** element identifies the delegate in a delegate access scenario.</span></span> 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 <span data-ttu-id="f6000-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="f6000-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6000-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f6000-106">Attributes and elements</span></span>

<span data-ttu-id="f6000-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f6000-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6000-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f6000-108">Attributes</span></span>

<span data-ttu-id="f6000-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f6000-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6000-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f6000-110">Child elements</span></span>

|<span data-ttu-id="f6000-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f6000-111">**Element**</span></span>|<span data-ttu-id="f6000-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f6000-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6000-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="f6000-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="f6000-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6000-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6000-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f6000-115">Parent elements</span></span>

|<span data-ttu-id="f6000-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f6000-116">**Element**</span></span>|<span data-ttu-id="f6000-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f6000-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6000-118">Message</span><span class="sxs-lookup"><span data-stu-id="f6000-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6000-119">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f6000-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f6000-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f6000-121">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-122">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="f6000-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f6000-123">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f6000-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f6000-125">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f6000-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f6000-127">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="f6000-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="f6000-129">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f6000-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f6000-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="f6000-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="f6000-131">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f6000-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f6000-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="f6000-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="f6000-133">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f6000-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f6000-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="f6000-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="f6000-135">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="f6000-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="f6000-137">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6000-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="f6000-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="f6000-139">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="f6000-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="f6000-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="f6000-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="f6000-141">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="f6000-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6000-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="f6000-142">Remarks</span></span>

<span data-ttu-id="f6000-143">L’élément **ReceivedRepresenting** est utilisé avec les éléments **from** et **ReceivedBy** dans les scénarios d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="f6000-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="f6000-144">Le tableau suivant répertorie les entités que ces éléments représentent dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="f6000-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="f6000-145">**Éléments dans un scénario d’accès délégué**</span><span class="sxs-lookup"><span data-stu-id="f6000-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="f6000-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f6000-146">**Element**</span></span>|<span data-ttu-id="f6000-147">**Entité représentée par l’élément**</span><span class="sxs-lookup"><span data-stu-id="f6000-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6000-148">From</span><span class="sxs-lookup"><span data-stu-id="f6000-148">From</span></span>](from.md) <br/> |<span data-ttu-id="f6000-149">Tierce partie</span><span class="sxs-lookup"><span data-stu-id="f6000-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="f6000-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="f6000-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="f6000-151">Délégué</span><span class="sxs-lookup"><span data-stu-id="f6000-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="f6000-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="f6000-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="f6000-153">Directeur</span><span class="sxs-lookup"><span data-stu-id="f6000-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="f6000-154">Dans un scénario d’accès délégué, si un tierce partie envoie une demande de réunion à un responsable qui a un délégué, le délégué verra une nouvelle demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f6000-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="f6000-155">Ces éléments permettent aux délégués de faire la distinction entre les messages qui leur sont envoyés directement et ceux qui leur sont envoyés en raison d’une règle de transfert de délégué.</span><span class="sxs-lookup"><span data-stu-id="f6000-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="f6000-156">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6000-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6000-157">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f6000-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6000-158">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f6000-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6000-159">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f6000-159">Schema Name</span></span>  <br/> |<span data-ttu-id="f6000-160">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f6000-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6000-161">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f6000-161">Validation File</span></span>  <br/> |<span data-ttu-id="f6000-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6000-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6000-163">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f6000-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6000-164">False</span><span class="sxs-lookup"><span data-stu-id="f6000-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6000-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f6000-165">See also</span></span>



- [<span data-ttu-id="f6000-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f6000-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

