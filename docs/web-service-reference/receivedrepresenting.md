---
title: ReceivedRepresenting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedRepresenting
api_type:
- schema
ms.assetid: 1157b042-6dce-4cdc-9700-e22b749da39f
description: L’élément ReceivedRepresenting identifie le principal dans un scénario d’accès délégué.
ms.openlocfilehash: f444fb88be9c0df174f0c1490cf7c499cc0c0539
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468221"
---
# <a name="receivedrepresenting"></a><span data-ttu-id="6cd00-103">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6cd00-103">ReceivedRepresenting</span></span>

<span data-ttu-id="6cd00-104">L’élément **ReceivedRepresenting** identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6cd00-104">The **ReceivedRepresenting** element identifies the principal in a delegate access scenario.</span></span> 
  
```xml
<ReceivedRepresenting>
   <Mailbox/>
</ReceivedRepresenting>
```

 <span data-ttu-id="6cd00-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="6cd00-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cd00-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6cd00-106">Attributes and elements</span></span>

<span data-ttu-id="6cd00-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6cd00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cd00-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6cd00-108">Attributes</span></span>

<span data-ttu-id="6cd00-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6cd00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cd00-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6cd00-110">Child elements</span></span>

|<span data-ttu-id="6cd00-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6cd00-111">**Element**</span></span>|<span data-ttu-id="6cd00-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6cd00-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cd00-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="6cd00-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="6cd00-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6cd00-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cd00-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6cd00-115">Parent elements</span></span>

|<span data-ttu-id="6cd00-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6cd00-116">**Element**</span></span>|<span data-ttu-id="6cd00-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6cd00-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cd00-118">Message</span><span class="sxs-lookup"><span data-stu-id="6cd00-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6cd00-119">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="6cd00-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6cd00-121">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-122">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="6cd00-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6cd00-123">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6cd00-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6cd00-125">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="6cd00-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6cd00-127">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="6cd00-129">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="6cd00-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="6cd00-131">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="6cd00-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="6cd00-133">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="6cd00-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="6cd00-135">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="6cd00-137">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="6cd00-139">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="6cd00-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="6cd00-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="6cd00-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="6cd00-141">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="6cd00-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6cd00-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="6cd00-142">Remarks</span></span>

<span data-ttu-id="6cd00-143">L’élément **ReceivedRepresenting** est utilisé avec les éléments **from** et **ReceivedBy** dans les scénarios d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6cd00-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="6cd00-144">Le tableau suivant répertorie les entités que ces éléments représentent dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6cd00-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="6cd00-145">**Éléments dans un scénario d’accès délégué**</span><span class="sxs-lookup"><span data-stu-id="6cd00-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="6cd00-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6cd00-146">**Element**</span></span>|<span data-ttu-id="6cd00-147">**Entité représentée par l’élément**</span><span class="sxs-lookup"><span data-stu-id="6cd00-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cd00-148">From</span><span class="sxs-lookup"><span data-stu-id="6cd00-148">From</span></span>](from.md) <br/> |<span data-ttu-id="6cd00-149">Tierce partie</span><span class="sxs-lookup"><span data-stu-id="6cd00-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="6cd00-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="6cd00-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6cd00-151">Délégué</span><span class="sxs-lookup"><span data-stu-id="6cd00-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="6cd00-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6cd00-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6cd00-153">Directeur</span><span class="sxs-lookup"><span data-stu-id="6cd00-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="6cd00-154">Dans un scénario d’accès délégué, si un tierce partie envoie une demande de réunion à un responsable qui a un délégué, le délégué verra une nouvelle demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="6cd00-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="6cd00-155">Ces éléments permettent aux délégués de faire la distinction entre les messages qui leur sont envoyés directement et ceux qui leur sont envoyés en raison d’une règle de transfert de délégué.</span><span class="sxs-lookup"><span data-stu-id="6cd00-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="6cd00-156">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cd00-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cd00-157">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6cd00-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cd00-158">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6cd00-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6cd00-159">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6cd00-159">Schema Name</span></span>  <br/> |<span data-ttu-id="6cd00-160">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6cd00-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="6cd00-161">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6cd00-161">Validation File</span></span>  <br/> |<span data-ttu-id="6cd00-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6cd00-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6cd00-163">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6cd00-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cd00-164">False</span><span class="sxs-lookup"><span data-stu-id="6cd00-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cd00-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6cd00-165">See also</span></span>



- [<span data-ttu-id="6cd00-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6cd00-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

