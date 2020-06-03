---
title: Pièces jointes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: L’élément Attachments contient les éléments ou les fichiers qui sont attachés à un élément dans la Banque d’Exchange.
ms.openlocfilehash: a9f79cd79f19e6226703c99c53c91efed600f495
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461533"
---
# <a name="attachments"></a><span data-ttu-id="4e848-103">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="4e848-103">Attachments</span></span>

<span data-ttu-id="4e848-104">L’élément **Attachments** contient les éléments ou les fichiers qui sont attachés à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="4e848-105">**ArrayOfAttachmentsType** et **NonEmptyArrayOfAttachmentsType**</span><span class="sxs-lookup"><span data-stu-id="4e848-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e848-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4e848-106">Attributes and elements</span></span>

<span data-ttu-id="4e848-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4e848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e848-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4e848-108">Attributes</span></span>

<span data-ttu-id="4e848-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4e848-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e848-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4e848-110">Child elements</span></span>

|<span data-ttu-id="4e848-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4e848-111">**Element**</span></span>|<span data-ttu-id="4e848-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4e848-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e848-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="4e848-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="4e848-114">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="4e848-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="4e848-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="4e848-116">Représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e848-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4e848-117">Parent elements</span></span>

|<span data-ttu-id="4e848-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4e848-118">**Element**</span></span>|<span data-ttu-id="4e848-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="4e848-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e848-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="4e848-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="4e848-121">Définit une demande de création d’une pièce jointe à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="4e848-122">Voici l’expression XPath de cet élément :`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="4e848-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="4e848-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="4e848-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="4e848-124">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e848-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="4e848-125">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4e848-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="4e848-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="4e848-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="4e848-127">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e848-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4e848-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="4e848-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="4e848-129">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e848-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4e848-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="4e848-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="4e848-131">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-132">Élément</span><span class="sxs-lookup"><span data-stu-id="4e848-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="4e848-133">Représente un élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="4e848-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="4e848-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="4e848-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="4e848-135">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-136">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="4e848-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4e848-137">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4e848-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4e848-139">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="4e848-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4e848-141">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-142">Message</span><span class="sxs-lookup"><span data-stu-id="4e848-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4e848-143">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="4e848-144">Tâche</span><span class="sxs-lookup"><span data-stu-id="4e848-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="4e848-145">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e848-146">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4e848-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4e848-147">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4e848-148">Contact</span><span class="sxs-lookup"><span data-stu-id="4e848-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4e848-149">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e848-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="4e848-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="4e848-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="4e848-151">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="4e848-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="4e848-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4e848-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="4e848-153">Contient l’État et le résultat d’une seule demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="4e848-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="4e848-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4e848-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="4e848-155">Contient l’État et le résultat d’une demande GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="4e848-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4e848-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="4e848-156">Remarks</span></span>

<span data-ttu-id="4e848-157">Les éléments **Attachments** ont les mêmes éléments enfants, mais sont basés sur différents types : **ArrayOfAttachmentsType** et **NonEmptyArrayOfAttachmentsType**.</span><span class="sxs-lookup"><span data-stu-id="4e848-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="4e848-158">Les types définissent si un élément enfant est requis.</span><span class="sxs-lookup"><span data-stu-id="4e848-158">The types define whether a child element is required.</span></span> <span data-ttu-id="4e848-159">Le **ArrayOfAttachmentsType** est utilisé uniquement dans le message de réponse.</span><span class="sxs-lookup"><span data-stu-id="4e848-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="4e848-160">Il est également important de noter que ces éléments se produisent dans les espaces de noms messages et types.</span><span class="sxs-lookup"><span data-stu-id="4e848-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="4e848-161">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4e848-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e848-162">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4e848-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e848-163">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4e848-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e848-164">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4e848-164">Schema Name</span></span>  <br/> |<span data-ttu-id="4e848-165">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4e848-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="4e848-166">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4e848-166">Validation File</span></span>  <br/> |<span data-ttu-id="4e848-167">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4e848-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e848-168">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4e848-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e848-169">False</span><span class="sxs-lookup"><span data-stu-id="4e848-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e848-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4e848-170">See also</span></span>

- [<span data-ttu-id="4e848-171">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4e848-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

