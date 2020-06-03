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
ms.openlocfilehash: 96070415c6d92a893f6c560884d9d191c7d5f15b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529503"
---
# <a name="bccrecipients"></a><span data-ttu-id="0f326-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="0f326-103">BccRecipients</span></span>

<span data-ttu-id="0f326-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **BccRecipients** représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d'un message électronique.</span><span class="sxs-lookup"><span data-stu-id="0f326-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="0f326-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="0f326-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f326-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f326-106">Attributes and elements</span></span>

<span data-ttu-id="0f326-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f326-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f326-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f326-108">Attributes</span></span>

<span data-ttu-id="0f326-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0f326-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f326-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f326-110">Child elements</span></span>

|<span data-ttu-id="0f326-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f326-111">**Element**</span></span>|<span data-ttu-id="0f326-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f326-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f326-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="0f326-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="0f326-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0f326-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f326-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f326-115">Parent elements</span></span>

|<span data-ttu-id="0f326-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f326-116">**Element**</span></span>|<span data-ttu-id="0f326-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f326-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f326-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0f326-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0f326-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-120">Message</span><span class="sxs-lookup"><span data-stu-id="0f326-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0f326-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0f326-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0f326-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0f326-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-124">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0f326-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0f326-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0f326-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0f326-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0f326-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0f326-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f326-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0f326-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="0f326-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f326-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f326-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0f326-133">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="0f326-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f326-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0f326-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0f326-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="0f326-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f326-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0f326-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0f326-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="0f326-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0f326-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f326-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f326-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0f326-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0f326-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="0f326-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0f326-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0f326-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0f326-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="0f326-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f326-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f326-144">Remarks</span></span>

<span data-ttu-id="0f326-p101">Impossible d'obtenir **BccRecipients** à l'aide d'une demande FindItem. Utilisez une demande de GetItem pour obtenir **BccRecipients**.</span><span class="sxs-lookup"><span data-stu-id="0f326-p101">You cannot get **BccRecipients** by using a FindItem request. Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="0f326-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0f326-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f326-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f326-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f326-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f326-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f326-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f326-150">Schema Name</span></span>  <br/> |<span data-ttu-id="0f326-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0f326-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f326-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f326-152">Validation File</span></span>  <br/> |<span data-ttu-id="0f326-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f326-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f326-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f326-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f326-155">False</span><span class="sxs-lookup"><span data-stu-id="0f326-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f326-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f326-156">See also</span></span>



- [<span data-ttu-id="0f326-157">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f326-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

