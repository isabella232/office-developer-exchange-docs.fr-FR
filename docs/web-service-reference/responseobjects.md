---
title: ResponseObjects
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: L’élément ResponseObjects contient une collection de tous les objets de réponse qui sont associés à un élément dans la banque d’informations Exchange.
ms.openlocfilehash: b1d95063439f5089665d2aad97d747665caef0ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829197"
---
# <a name="responseobjects"></a><span data-ttu-id="a3f52-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="a3f52-103">ResponseObjects</span></span>

<span data-ttu-id="a3f52-104">L’élément **ResponseObjects** contient une collection de tous les objets de réponse qui sont associés à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 <span data-ttu-id="a3f52-105">**NonEmptyArrayOfResponseObjectsType**</span><span class="sxs-lookup"><span data-stu-id="a3f52-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3f52-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a3f52-106">Attributes and elements</span></span>

<span data-ttu-id="a3f52-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a3f52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3f52-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a3f52-108">Attributes</span></span>

<span data-ttu-id="a3f52-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3f52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3f52-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a3f52-110">Child elements</span></span>

|<span data-ttu-id="a3f52-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3f52-111">**Element**</span></span>|<span data-ttu-id="a3f52-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3f52-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3f52-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="a3f52-114">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="a3f52-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="a3f52-116">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="a3f52-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="a3f52-118">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="a3f52-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="a3f52-120">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-121">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="a3f52-122">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="a3f52-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-123">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="a3f52-124">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="a3f52-126">Représente l’objet réponse utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="a3f52-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="a3f52-128">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="a3f52-130">Contient une réponse à un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="a3f52-130">Contains a reply to a post item.</span></span> <span data-ttu-id="a3f52-131">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a3f52-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="a3f52-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="a3f52-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="a3f52-133">Permet de supprimer les demandes de confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="a3f52-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-134">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="a3f52-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="a3f52-135">Utilisé pour accepter une invitation qui permet d’accéder aux données de contacts ou de calendrier d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a3f52-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3f52-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a3f52-136">Parent elements</span></span>

|<span data-ttu-id="a3f52-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3f52-137">**Element**</span></span>|<span data-ttu-id="a3f52-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3f52-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3f52-139">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a3f52-140">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-141">Contact</span><span class="sxs-lookup"><span data-stu-id="a3f52-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a3f52-142">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="a3f52-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="a3f52-144">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="a3f52-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-145">Élément</span><span class="sxs-lookup"><span data-stu-id="a3f52-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="a3f52-146">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="a3f52-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="a3f52-148">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="a3f52-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="a3f52-150">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a3f52-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a3f52-152">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a3f52-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="a3f52-154">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-155">Message</span><span class="sxs-lookup"><span data-stu-id="a3f52-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a3f52-156">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="a3f52-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="a3f52-158">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3f52-159">Tâche</span><span class="sxs-lookup"><span data-stu-id="a3f52-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="a3f52-160">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3f52-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="a3f52-161">Remarks</span></span>

<span data-ttu-id="a3f52-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3f52-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3f52-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a3f52-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3f52-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a3f52-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3f52-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a3f52-165">Schema Name</span></span>  <br/> |<span data-ttu-id="a3f52-166">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a3f52-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3f52-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a3f52-167">Validation File</span></span>  <br/> |<span data-ttu-id="a3f52-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3f52-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3f52-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a3f52-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3f52-170">False</span><span class="sxs-lookup"><span data-stu-id="a3f52-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3f52-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a3f52-171">See also</span></span>



- [<span data-ttu-id="a3f52-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a3f52-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

