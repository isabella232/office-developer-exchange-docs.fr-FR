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
ms.openlocfilehash: 45ad76d19bd43e2081aa9b9eb63547e091014803
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462254"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="dde51-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="dde51-103">CancelCalendarItem</span></span>

<span data-ttu-id="dde51-104">L’élément **CancelCalendarItem** représente l’objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="dde51-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
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

 <span data-ttu-id="dde51-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="dde51-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dde51-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dde51-106">Attributes and elements</span></span>

<span data-ttu-id="dde51-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dde51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dde51-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dde51-108">Attributes</span></span>

<span data-ttu-id="dde51-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dde51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dde51-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dde51-110">Child elements</span></span>

|<span data-ttu-id="dde51-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dde51-111">**Element**</span></span>|<span data-ttu-id="dde51-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dde51-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dde51-113">Subject</span><span class="sxs-lookup"><span data-stu-id="dde51-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="dde51-114">Représente la propriété Subject des éléments de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="dde51-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="dde51-115">Corps</span><span class="sxs-lookup"><span data-stu-id="dde51-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="dde51-116">Non utilisé par **CancelCalendarItem**.</span><span class="sxs-lookup"><span data-stu-id="dde51-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="dde51-117">Utilisez la propriété [NewBodyContent](newbodycontent.md) pour définir le contenu du corps.</span><span class="sxs-lookup"><span data-stu-id="dde51-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="dde51-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="dde51-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="dde51-119">Contient un ensemble de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="dde51-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="dde51-120">Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="dde51-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="dde51-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="dde51-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="dde51-122">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="dde51-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="dde51-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="dde51-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="dde51-124">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="dde51-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="dde51-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dde51-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="dde51-126">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="dde51-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="dde51-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dde51-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="dde51-128">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="dde51-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="dde51-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="dde51-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="dde51-130">Identifie l’élément auquel l’objet de réponse fait référence.</span><span class="sxs-lookup"><span data-stu-id="dde51-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="dde51-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="dde51-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="dde51-132">Représente le nouveau contenu du corps d’un message.</span><span class="sxs-lookup"><span data-stu-id="dde51-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="dde51-133">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="dde51-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="dde51-134">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="dde51-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="dde51-135">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dde51-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="dde51-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="dde51-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="dde51-137">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="dde51-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="dde51-138">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dde51-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dde51-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dde51-139">Parent elements</span></span>

|<span data-ttu-id="dde51-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dde51-140">**Element**</span></span>|<span data-ttu-id="dde51-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="dde51-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dde51-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="dde51-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="dde51-143">Décrit tous les éléments adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="dde51-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="dde51-144">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="dde51-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="dde51-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="dde51-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="dde51-146">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="dde51-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="dde51-147">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="dde51-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="dde51-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="dde51-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="dde51-149">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="dde51-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dde51-150">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="dde51-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="dde51-151">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="dde51-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dde51-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="dde51-152">Remarks</span></span>

<span data-ttu-id="dde51-153">L’élément **CancelCalendarItem** est affiché uniquement par l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="dde51-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="dde51-154">Elle s’applique uniquement à l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="dde51-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="dde51-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dde51-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dde51-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dde51-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dde51-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dde51-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dde51-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dde51-158">Schema Name</span></span>  <br/> |<span data-ttu-id="dde51-159">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dde51-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="dde51-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dde51-160">Validation File</span></span>  <br/> |<span data-ttu-id="dde51-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dde51-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dde51-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dde51-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="dde51-163">False</span><span class="sxs-lookup"><span data-stu-id="dde51-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dde51-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dde51-164">See also</span></span>

- [<span data-ttu-id="dde51-165">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dde51-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

