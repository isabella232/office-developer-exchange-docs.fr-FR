---
title: ReplyAllToItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyAllToItem
api_type:
- schema
ms.assetid: 8ca970ca-ca73-40db-9233-7b271cc5f44f
description: L’élément ReplyToAllItem contient une réponse à l’expéditeur et à tous les destinataires identifiés d’un élément dans la Banque d’Exchange.
ms.openlocfilehash: fd32aba84448728985d66edd03d378de2b0b3564
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457472"
---
# <a name="replyalltoitem"></a><span data-ttu-id="2595f-103">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="2595f-103">ReplyAllToItem</span></span>

<span data-ttu-id="2595f-104">L’élément **ReplyToAllItem** contient une réponse à l’expéditeur et à tous les destinataires identifiés d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="2595f-104">The **ReplyToAllItem** element contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span> 
  
```xml
<ReplyAllToItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <From/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</ReplyAllToItem>
```

 <span data-ttu-id="2595f-105">**ReplyAllToItemType**</span><span class="sxs-lookup"><span data-stu-id="2595f-105">**ReplyAllToItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2595f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2595f-106">Attributes and elements</span></span>

<span data-ttu-id="2595f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2595f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2595f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2595f-108">Attributes</span></span>

<span data-ttu-id="2595f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2595f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2595f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2595f-110">Child elements</span></span>

|<span data-ttu-id="2595f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2595f-111">**Element**</span></span>|<span data-ttu-id="2595f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2595f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2595f-113">Subject</span><span class="sxs-lookup"><span data-stu-id="2595f-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="2595f-114">Représente la propriété Subject des éléments de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="2595f-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="2595f-115">Body</span><span class="sxs-lookup"><span data-stu-id="2595f-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="2595f-116">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="2595f-116">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="2595f-117">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="2595f-117">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="2595f-118">Contient un ensemble de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="2595f-118">Contains a set of recipients of an item.</span></span> <span data-ttu-id="2595f-119">Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="2595f-119">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="2595f-120">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="2595f-120">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="2595f-121">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="2595f-121">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="2595f-122">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="2595f-122">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="2595f-123">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="2595f-123">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2595f-124">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2595f-124">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="2595f-125">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="2595f-125">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="2595f-126">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2595f-126">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="2595f-127">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="2595f-127">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="2595f-128">From</span><span class="sxs-lookup"><span data-stu-id="2595f-128">From</span></span>](from.md) <br/> |<span data-ttu-id="2595f-129">Représente l’adresse à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="2595f-129">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="2595f-130">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="2595f-130">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="2595f-131">Identifie l’élément auquel l’objet de réponse fait référence.</span><span class="sxs-lookup"><span data-stu-id="2595f-131">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="2595f-132">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="2595f-132">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="2595f-133">Représente le nouveau contenu du corps d’un message.</span><span class="sxs-lookup"><span data-stu-id="2595f-133">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="2595f-134">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="2595f-134">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="2595f-135">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="2595f-135">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="2595f-136">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2595f-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="2595f-137">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="2595f-137">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="2595f-138">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="2595f-138">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="2595f-139">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2595f-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2595f-140">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2595f-140">Parent elements</span></span>

|<span data-ttu-id="2595f-141">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2595f-141">**Element**</span></span>|<span data-ttu-id="2595f-142">**Description**</span><span class="sxs-lookup"><span data-stu-id="2595f-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2595f-143">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="2595f-143">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="2595f-144">Décrit tous les éléments adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="2595f-144">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="2595f-145">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2595f-145">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="2595f-146">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="2595f-146">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="2595f-147">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="2595f-147">Describes all items that conflict with a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="2595f-148">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2595f-148">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="2595f-149">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="2595f-149">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="2595f-150">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2595f-150">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2595f-151">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="2595f-151">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="2595f-152">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="2595f-152">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2595f-153">Remarques</span><span class="sxs-lookup"><span data-stu-id="2595f-153">Remarks</span></span>

<span data-ttu-id="2595f-154">L’élément [from](from.md) doit être défini sur l’adresse de messagerie du principal si un élément est une réponse d’un délégué.</span><span class="sxs-lookup"><span data-stu-id="2595f-154">The [From](from.md) element should be set to the e-mail address of the principal if an item is a reply by a delegate.</span></span> <span data-ttu-id="2595f-155">Si le délégué ne définit pas la propriété [from](from.md) , l’élément semble avoir été envoyé directement à partir de la boîte aux lettres du délégué.</span><span class="sxs-lookup"><span data-stu-id="2595f-155">If the delegate does not set the [From](from.md) property, the item will appear to have been sent directly from the delegate's mailbox.</span></span> 
  
<span data-ttu-id="2595f-156">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2595f-156">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2595f-157">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2595f-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2595f-158">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2595f-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2595f-159">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2595f-159">Schema Name</span></span>  <br/> |<span data-ttu-id="2595f-160">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2595f-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="2595f-161">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2595f-161">Validation File</span></span>  <br/> |<span data-ttu-id="2595f-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2595f-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2595f-163">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2595f-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="2595f-164">False</span><span class="sxs-lookup"><span data-stu-id="2595f-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2595f-165">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2595f-165">See also</span></span>

- [<span data-ttu-id="2595f-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2595f-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

