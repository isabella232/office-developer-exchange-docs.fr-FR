---
title: DeclineItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeclineItem
api_type:
- schema
ms.assetid: 2d8d2389-924e-4d03-a324-35d56cf0d6b1
description: L’élément DeclineItem représente une réponse de refus à une demande de réunion.
ms.openlocfilehash: d7076708248bf1ddc0472b802e4de94a436dcde8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755835"
---
# <a name="declineitem"></a><span data-ttu-id="23482-103">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="23482-103">DeclineItem</span></span>

<span data-ttu-id="23482-104">L’élément **DeclineItem** représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="23482-104">The **DeclineItem** element represents a Decline reply to a meeting request.</span></span> 
  
```xml
<DeclineItem>
   <ItemClass/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <InternetMessageHeaders/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <ProposedStart/>
   <ProposedEnd/>
</DeclineItem>
```

<span data-ttu-id="23482-105">**DeclineItemType**</span><span class="sxs-lookup"><span data-stu-id="23482-105">**DeclineItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="23482-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="23482-106">Attributes and elements</span></span>

<span data-ttu-id="23482-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="23482-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23482-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="23482-108">Attributes</span></span>

<span data-ttu-id="23482-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="23482-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23482-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="23482-110">Child elements</span></span>

|<span data-ttu-id="23482-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="23482-111">**Element**</span></span>|<span data-ttu-id="23482-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="23482-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23482-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="23482-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="23482-114">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="23482-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="23482-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="23482-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="23482-116">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="23482-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="23482-117">Corps</span><span class="sxs-lookup"><span data-stu-id="23482-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="23482-118">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="23482-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="23482-119">Attachments</span><span class="sxs-lookup"><span data-stu-id="23482-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="23482-120">Contient l’élément ou un fichier joint à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="23482-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="23482-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="23482-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="23482-122">Représente le nom d’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes.</span><span class="sxs-lookup"><span data-stu-id="23482-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="23482-123">Sender</span><span class="sxs-lookup"><span data-stu-id="23482-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="23482-124">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="23482-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="23482-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="23482-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="23482-126">Contient un ensemble de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="23482-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="23482-127">Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="23482-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="23482-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="23482-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="23482-129">Représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="23482-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="23482-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="23482-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="23482-131">Représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="23482-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="23482-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="23482-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="23482-133">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="23482-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="23482-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="23482-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="23482-135">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="23482-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="23482-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="23482-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="23482-137">Identifie l’élément auquel fait référence l’objet de réponse.</span><span class="sxs-lookup"><span data-stu-id="23482-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="23482-138">Reçu par</span><span class="sxs-lookup"><span data-stu-id="23482-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="23482-139">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="23482-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="23482-140">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="23482-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="23482-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="23482-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="23482-142">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="23482-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="23482-143">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="23482-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="23482-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="23482-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="23482-145">Spécifie l’heure de début proposée de la réunion.</span><span class="sxs-lookup"><span data-stu-id="23482-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="23482-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="23482-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="23482-147">Spécifie l’heure de fin proposée de la réunion.</span><span class="sxs-lookup"><span data-stu-id="23482-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23482-148">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="23482-148">Parent elements</span></span>

|<span data-ttu-id="23482-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="23482-149">**Element**</span></span>|<span data-ttu-id="23482-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="23482-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23482-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="23482-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="23482-152">Décrit tous les éléments qui sont adjacentes à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="23482-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/><span data-ttu-id="23482-153">Voici quelques-unes des expressions XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="23482-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="23482-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="23482-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="23482-155">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="23482-155">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="23482-156">Voici quelques-unes des expressions XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="23482-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="23482-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="23482-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="23482-158">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="23482-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="23482-159">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="23482-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="23482-160">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="23482-160">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23482-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="23482-161">Remarks</span></span>

<span data-ttu-id="23482-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS du serveur Exchange qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="23482-162">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23482-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="23482-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23482-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="23482-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23482-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="23482-165">Schema Name</span></span>  <br/> |<span data-ttu-id="23482-166">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="23482-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="23482-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="23482-167">Validation File</span></span>  <br/> |<span data-ttu-id="23482-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="23482-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23482-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="23482-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="23482-170">False</span><span class="sxs-lookup"><span data-stu-id="23482-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23482-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="23482-171">See also</span></span>

- [<span data-ttu-id="23482-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23482-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

