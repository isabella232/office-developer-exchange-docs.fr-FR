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
ms.openlocfilehash: a3fb2b62ea2fa895a664034d2150f46a3099f6c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457430"
---
# <a name="declineitem"></a><span data-ttu-id="f2cb7-103">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="f2cb7-103">DeclineItem</span></span>

<span data-ttu-id="f2cb7-104">L’élément **DeclineItem** représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-104">The **DeclineItem** element represents a Decline reply to a meeting request.</span></span> 
  
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

<span data-ttu-id="f2cb7-105">**DeclineItemType**</span><span class="sxs-lookup"><span data-stu-id="f2cb7-105">**DeclineItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f2cb7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f2cb7-106">Attributes and elements</span></span>

<span data-ttu-id="f2cb7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2cb7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f2cb7-108">Attributes</span></span>

<span data-ttu-id="f2cb7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2cb7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f2cb7-110">Child elements</span></span>

|<span data-ttu-id="f2cb7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2cb7-111">**Element**</span></span>|<span data-ttu-id="f2cb7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2cb7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2cb7-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="f2cb7-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="f2cb7-114">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="f2cb7-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="f2cb7-116">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-117">Body</span><span class="sxs-lookup"><span data-stu-id="f2cb7-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="f2cb7-118">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-119">Attachments</span><span class="sxs-lookup"><span data-stu-id="f2cb7-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f2cb7-120">Contient l’élément ou le fichier qui est associé à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="f2cb7-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="f2cb7-122">Représente le nom de l’en-tête de message Internet d’un en-tête donné dans la collection headers.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-123">Sender</span><span class="sxs-lookup"><span data-stu-id="f2cb7-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="f2cb7-124">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="f2cb7-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="f2cb7-126">Contient un ensemble de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="f2cb7-127">Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="f2cb7-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="f2cb7-129">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="f2cb7-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="f2cb7-131">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f2cb7-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="f2cb7-133">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f2cb7-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="f2cb7-135">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="f2cb7-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="f2cb7-137">Identifie l’élément auquel l’objet de réponse fait référence.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="f2cb7-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="f2cb7-139">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="f2cb7-140">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f2cb7-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="f2cb7-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="f2cb7-142">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="f2cb7-143">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="f2cb7-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="f2cb7-145">Spécifie l’heure de début proposée de la réunion.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="f2cb7-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="f2cb7-147">Spécifie l’heure de fin proposée de la réunion.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2cb7-148">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f2cb7-148">Parent elements</span></span>

|<span data-ttu-id="f2cb7-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2cb7-149">**Element**</span></span>|<span data-ttu-id="f2cb7-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2cb7-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2cb7-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="f2cb7-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="f2cb7-152">Décrit tous les éléments adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/><span data-ttu-id="f2cb7-153">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f2cb7-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="f2cb7-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="f2cb7-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="f2cb7-155">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-155">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="f2cb7-156">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f2cb7-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="f2cb7-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="f2cb7-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="f2cb7-158">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f2cb7-159">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="f2cb7-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="f2cb7-160">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="f2cb7-160">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2cb7-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="f2cb7-161">Remarks</span></span>

<span data-ttu-id="f2cb7-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS du serveur Exchange sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f2cb7-162">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2cb7-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f2cb7-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2cb7-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f2cb7-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2cb7-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f2cb7-165">Schema Name</span></span>  <br/> |<span data-ttu-id="f2cb7-166">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f2cb7-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2cb7-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f2cb7-167">Validation File</span></span>  <br/> |<span data-ttu-id="f2cb7-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2cb7-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2cb7-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f2cb7-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2cb7-170">False</span><span class="sxs-lookup"><span data-stu-id="f2cb7-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2cb7-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f2cb7-171">See also</span></span>

- [<span data-ttu-id="f2cb7-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f2cb7-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

