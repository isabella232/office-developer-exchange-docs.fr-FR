---
title: Éléments (NonEmptyArrayOfAllItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: d61ef1cc-ddfc-480a-9625-7b436cb33ae0
description: L’élément ITEMS contient un ensemble d’éléments à créer.
ms.openlocfilehash: 0f70f1fe4348b5b74cef6be6414618af1e3de260
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459853"
---
# <a name="items-nonemptyarrayofallitemstype"></a><span data-ttu-id="aceec-103">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="aceec-103">Items (NonEmptyArrayOfAllItemsType)</span></span>

<span data-ttu-id="aceec-104">L’élément **Items** contient un ensemble d’éléments à créer.</span><span class="sxs-lookup"><span data-stu-id="aceec-104">The **Items** element contains a set of items to create.</span></span> 
  
```XML
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</Items>
```

 <span data-ttu-id="aceec-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="aceec-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aceec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aceec-106">Attributes and elements</span></span>

<span data-ttu-id="aceec-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aceec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aceec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aceec-108">Attributes</span></span>

<span data-ttu-id="aceec-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="aceec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aceec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aceec-110">Child elements</span></span>

|<span data-ttu-id="aceec-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aceec-111">**Element**</span></span>|<span data-ttu-id="aceec-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aceec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aceec-113">Élément</span><span class="sxs-lookup"><span data-stu-id="aceec-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="aceec-114">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-115">Message</span><span class="sxs-lookup"><span data-stu-id="aceec-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aceec-116">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-116">Represents an Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="aceec-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="aceec-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="aceec-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="aceec-119">Contact</span><span class="sxs-lookup"><span data-stu-id="aceec-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="aceec-120">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="aceec-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="aceec-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="aceec-122">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="aceec-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="aceec-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="aceec-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="aceec-124">Représente un message de réunion dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-125">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="aceec-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="aceec-126">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="aceec-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="aceec-128">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="aceec-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="aceec-130">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-131">Tâche</span><span class="sxs-lookup"><span data-stu-id="aceec-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="aceec-132">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="aceec-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="aceec-134">Contient une réponse à l’expéditeur d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-134">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-135">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="aceec-135">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="aceec-136">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="aceec-136">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="aceec-137">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="aceec-137">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="aceec-138">Contient une réponse à l’expéditeur et à tous les destinataires identifiés d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-138">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aceec-139">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="aceec-139">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="aceec-140">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="aceec-140">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aceec-141">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="aceec-141">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="aceec-142">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="aceec-142">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aceec-143">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="aceec-143">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="aceec-144">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="aceec-144">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aceec-145">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="aceec-145">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="aceec-146">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="aceec-146">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="aceec-147">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="aceec-147">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="aceec-148">Représente un objet Response qui est utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation.</span><span class="sxs-lookup"><span data-stu-id="aceec-148">Represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span>  <br/> |
|[<span data-ttu-id="aceec-149">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="aceec-149">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="aceec-150">Contient une réponse à un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="aceec-150">Contains a reply to a post item.</span></span>  <br/> |
|[<span data-ttu-id="aceec-151">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="aceec-151">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="aceec-152">Permet de supprimer les confirmations de lecture.</span><span class="sxs-lookup"><span data-stu-id="aceec-152">Used to suppress read receipts.</span></span>  <br/> |
|[<span data-ttu-id="aceec-153">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="aceec-153">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="aceec-154">Permet d’accepter une invitation qui autorise l’accès au calendrier ou aux données de contacts d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="aceec-154">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aceec-155">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aceec-155">Parent elements</span></span>

|<span data-ttu-id="aceec-156">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aceec-156">**Element**</span></span>|<span data-ttu-id="aceec-157">**Description**</span><span class="sxs-lookup"><span data-stu-id="aceec-157">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aceec-158">CreateItem</span><span class="sxs-lookup"><span data-stu-id="aceec-158">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="aceec-159">Définit la demande de création d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-159">Defines the request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="aceec-160">Voici l’expression XPath de cet élément :`/CreateItem`</span><span class="sxs-lookup"><span data-stu-id="aceec-160">The following is the XPath expression to this element:  `/CreateItem`</span></span> <br/> |
|[<span data-ttu-id="aceec-161">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="aceec-161">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="aceec-162">Identifie un nœud unique dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="aceec-162">Identifies a single node in a conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aceec-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="aceec-163">Remarks</span></span>

<span data-ttu-id="aceec-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aceec-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aceec-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aceec-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aceec-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aceec-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aceec-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aceec-167">Schema Name</span></span>  <br/> |<span data-ttu-id="aceec-168">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="aceec-168">Message schema</span></span>  <br/> |
|<span data-ttu-id="aceec-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aceec-169">Validation File</span></span>  <br/> |<span data-ttu-id="aceec-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aceec-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aceec-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aceec-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="aceec-172">False</span><span class="sxs-lookup"><span data-stu-id="aceec-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aceec-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aceec-173">See also</span></span>



[<span data-ttu-id="aceec-174">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="aceec-174">CreateFolder operation</span></span>](createfolder-operation.md)
  
[<span data-ttu-id="aceec-175">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="aceec-175">CreateItem operation</span></span>](createitem-operation.md)


[<span data-ttu-id="aceec-176">Création de dossiers (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="aceec-176">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

