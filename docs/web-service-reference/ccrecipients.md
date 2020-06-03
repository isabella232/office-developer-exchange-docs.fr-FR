---
title: CcRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CcRecipients
api_type:
- schema
ms.assetid: 5c20ec3a-0bee-4e67-b220-586ed0d601c9
description: L'élément CcRecipients représente une collection de destinataires qui reçoivent une copie du message.
ms.openlocfilehash: 57d0e2d3b2c44fbd7bb30696002b27e83d1e274e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462205"
---
# <a name="ccrecipients"></a><span data-ttu-id="f45bf-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="f45bf-103">CcRecipients</span></span>

<span data-ttu-id="f45bf-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **CcRecipients** représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="f45bf-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="f45bf-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="f45bf-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f45bf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f45bf-106">Attributes and elements</span></span>

<span data-ttu-id="f45bf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f45bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f45bf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f45bf-108">Attributes</span></span>

<span data-ttu-id="f45bf-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f45bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f45bf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f45bf-110">Child elements</span></span>

|<span data-ttu-id="f45bf-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f45bf-111">**Element**</span></span>|<span data-ttu-id="f45bf-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f45bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f45bf-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="f45bf-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="f45bf-114">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f45bf-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f45bf-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f45bf-115">Parent elements</span></span>

|<span data-ttu-id="f45bf-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f45bf-116">**Element**</span></span>|<span data-ttu-id="f45bf-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f45bf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f45bf-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="f45bf-119">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-120">Message</span><span class="sxs-lookup"><span data-stu-id="f45bf-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f45bf-121">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f45bf-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f45bf-123">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-124">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="f45bf-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f45bf-125">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f45bf-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f45bf-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f45bf-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f45bf-129">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="f45bf-131">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f45bf-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="f45bf-133">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f45bf-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="f45bf-135">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f45bf-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="f45bf-137">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="f45bf-139">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f45bf-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="f45bf-141">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="f45bf-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="f45bf-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="f45bf-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="f45bf-143">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="f45bf-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f45bf-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="f45bf-144">Remarks</span></span>

<span data-ttu-id="f45bf-p101">Impossible d'obtenir **CcRecipients** à l'aide d'une demande FindItem. Utilisez une demande de GetItem pour obtenir **CcRecipients**.</span><span class="sxs-lookup"><span data-stu-id="f45bf-p101">You cannot get **CcRecipients** by using a FindItem request. Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="f45bf-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f45bf-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f45bf-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f45bf-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f45bf-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f45bf-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f45bf-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f45bf-150">Schema Name</span></span>  <br/> |<span data-ttu-id="f45bf-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f45bf-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="f45bf-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f45bf-152">Validation File</span></span>  <br/> |<span data-ttu-id="f45bf-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f45bf-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f45bf-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f45bf-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="f45bf-155">False</span><span class="sxs-lookup"><span data-stu-id="f45bf-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f45bf-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f45bf-156">See also</span></span>



- [<span data-ttu-id="f45bf-157">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f45bf-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

