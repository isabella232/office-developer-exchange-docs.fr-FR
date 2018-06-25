---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: L'élément BccRecipients représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d'un message électronique.
ms.openlocfilehash: 858fe74c32cb7d1ed624888c06bba4ffe09d489e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755379"
---
# <a name="bccrecipients"></a><span data-ttu-id="3e350-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="3e350-103">BccRecipients</span></span>

<span data-ttu-id="3e350-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **BccRecipients** représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d'un message électronique.</span><span class="sxs-lookup"><span data-stu-id="3e350-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="3e350-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="3e350-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e350-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e350-106">Attributes and elements</span></span>

<span data-ttu-id="3e350-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e350-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e350-108">Attributes</span></span>

<span data-ttu-id="3e350-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e350-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e350-110">Child elements</span></span>

|<span data-ttu-id="3e350-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e350-111">**Element**</span></span>|<span data-ttu-id="3e350-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e350-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e350-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="3e350-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3e350-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e350-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e350-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e350-115">Parent elements</span></span>

|<span data-ttu-id="3e350-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e350-116">**Element**</span></span>|<span data-ttu-id="3e350-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e350-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e350-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="3e350-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="3e350-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-120">Message</span><span class="sxs-lookup"><span data-stu-id="3e350-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3e350-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="3e350-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="3e350-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="3e350-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3e350-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3e350-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="3e350-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="3e350-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="3e350-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="3e350-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="3e350-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="3e350-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="3e350-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3e350-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="3e350-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="3e350-133">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="3e350-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3e350-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="3e350-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="3e350-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="3e350-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3e350-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="3e350-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="3e350-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="3e350-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="3e350-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e350-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e350-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="3e350-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="3e350-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="3e350-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="3e350-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="3e350-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="3e350-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="3e350-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3e350-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e350-144">Remarks</span></span>

<span data-ttu-id="3e350-p101">Impossible d'obtenir **BccRecipients** à l'aide d'une demande FindItem. Utilisez une demande de GetItem pour obtenir **BccRecipients**.</span><span class="sxs-lookup"><span data-stu-id="3e350-p101">You cannot get **BccRecipients** by using a FindItem request. Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="3e350-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3e350-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e350-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e350-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e350-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e350-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e350-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e350-150">Schema Name</span></span>  <br/> |<span data-ttu-id="3e350-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3e350-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e350-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e350-152">Validation File</span></span>  <br/> |<span data-ttu-id="3e350-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e350-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e350-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e350-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e350-155">False</span><span class="sxs-lookup"><span data-stu-id="3e350-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e350-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e350-156">See also</span></span>



- [<span data-ttu-id="3e350-157">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e350-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

