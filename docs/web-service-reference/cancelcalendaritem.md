---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: L’élément CancelCalendarItem représente l’objet de réponse qui est utilisé pour annuler une réunion.
ms.openlocfilehash: 262f60db33abac36156b069dc85e1fccb3522d5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755490"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="a62f3-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="a62f3-103">CancelCalendarItem</span></span>

<span data-ttu-id="a62f3-104">L’élément **CancelCalendarItem** représente l’objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="a62f3-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 <span data-ttu-id="a62f3-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="a62f3-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a62f3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a62f3-106">Attributes and elements</span></span>

<span data-ttu-id="a62f3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a62f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a62f3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a62f3-108">Attributes</span></span>

<span data-ttu-id="a62f3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a62f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a62f3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a62f3-110">Child elements</span></span>

|<span data-ttu-id="a62f3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a62f3-111">**Element**</span></span>|<span data-ttu-id="a62f3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a62f3-113">Objet</span><span class="sxs-lookup"><span data-stu-id="a62f3-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="a62f3-114">Représente la propriété subject d’éléments de banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="a62f3-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-115">Corps</span><span class="sxs-lookup"><span data-stu-id="a62f3-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="a62f3-116">Non utilisé par **CancelCalendarItem**.</span><span class="sxs-lookup"><span data-stu-id="a62f3-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="a62f3-117">Utilisez la propriété [NewBodyContent](newbodycontent.md) pour définir le contenu du corps.</span><span class="sxs-lookup"><span data-stu-id="a62f3-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="a62f3-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="a62f3-119">Contient un ensemble de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="a62f3-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="a62f3-120">Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="a62f3-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="a62f3-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="a62f3-122">Représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="a62f3-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="a62f3-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="a62f3-124">Représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="a62f3-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a62f3-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="a62f3-126">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="a62f3-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a62f3-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="a62f3-128">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="a62f3-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="a62f3-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="a62f3-130">Identifie l’élément auquel fait référence l’objet de réponse.</span><span class="sxs-lookup"><span data-stu-id="a62f3-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="a62f3-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="a62f3-132">Représente le nouveau contenu du corps d’un message.</span><span class="sxs-lookup"><span data-stu-id="a62f3-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-133">Reçu par</span><span class="sxs-lookup"><span data-stu-id="a62f3-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="a62f3-134">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="a62f3-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="a62f3-135">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a62f3-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="a62f3-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="a62f3-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="a62f3-137">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="a62f3-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="a62f3-138">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a62f3-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a62f3-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a62f3-139">Parent elements</span></span>

|<span data-ttu-id="a62f3-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a62f3-140">**Element**</span></span>|<span data-ttu-id="a62f3-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62f3-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a62f3-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="a62f3-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="a62f3-143">Décrit tous les éléments qui sont adjacentes à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="a62f3-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="a62f3-144">Voici quelques-unes des expressions XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a62f3-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="a62f3-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="a62f3-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="a62f3-146">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="a62f3-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="a62f3-147">Voici quelques-unes des expressions XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a62f3-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="a62f3-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="a62f3-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="a62f3-149">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a62f3-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a62f3-150">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a62f3-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="a62f3-151">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="a62f3-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a62f3-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="a62f3-152">Remarks</span></span>

<span data-ttu-id="a62f3-153">L’élément **CancelCalendarItem** est affichée uniquement par l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="a62f3-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="a62f3-154">Elle s’applique uniquement à l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="a62f3-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="a62f3-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a62f3-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a62f3-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a62f3-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a62f3-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a62f3-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a62f3-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a62f3-158">Schema Name</span></span>  <br/> |<span data-ttu-id="a62f3-159">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a62f3-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="a62f3-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a62f3-160">Validation File</span></span>  <br/> |<span data-ttu-id="a62f3-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a62f3-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a62f3-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a62f3-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="a62f3-163">False</span><span class="sxs-lookup"><span data-stu-id="a62f3-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a62f3-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a62f3-164">See also</span></span>

- [<span data-ttu-id="a62f3-165">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a62f3-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

