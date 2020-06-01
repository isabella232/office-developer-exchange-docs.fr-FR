---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: L'élément ToRecipients contient un tableau de destinataires d'un élément. Voici les principaux destinataires d'un élément.
ms.openlocfilehash: 39ee359e1eaf3d0b6455fb1734222e78054dc7f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467542"
---
# <a name="torecipients"></a><span data-ttu-id="0bad3-104">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="0bad3-104">ToRecipients</span></span>

<span data-ttu-id="0bad3-p102">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **ToRecipients** contient un tableau de destinataires d'un élément. Voici les principaux destinataires d'un élément.</span><span class="sxs-lookup"><span data-stu-id="0bad3-p102">The **ToRecipients** element contains an array of recipients of an item. These are the primary recipients of an item.</span></span> 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 <span data-ttu-id="0bad3-107">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="0bad3-107">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bad3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0bad3-108">Attributes and elements</span></span>

<span data-ttu-id="0bad3-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0bad3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bad3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0bad3-110">Attributes</span></span>

<span data-ttu-id="0bad3-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0bad3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bad3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0bad3-112">Child elements</span></span>

|<span data-ttu-id="0bad3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0bad3-113">**Element**</span></span>|<span data-ttu-id="0bad3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0bad3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bad3-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="0bad3-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="0bad3-116">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bad3-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bad3-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0bad3-117">Parent elements</span></span>

|<span data-ttu-id="0bad3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0bad3-118">**Element**</span></span>|<span data-ttu-id="0bad3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0bad3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bad3-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0bad3-121">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-122">Message</span><span class="sxs-lookup"><span data-stu-id="0bad3-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0bad3-123">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-124">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0bad3-124">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0bad3-125">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-125">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-126">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0bad3-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0bad3-127">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-128">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0bad3-128">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0bad3-129">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-129">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0bad3-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0bad3-131">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-132">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-132">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0bad3-133">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="0bad3-133">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-134">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-134">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0bad3-135">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="0bad3-135">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-136">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-136">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0bad3-137">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="0bad3-137">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-138">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-138">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0bad3-139">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-139">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-140">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-140">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0bad3-141">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bad3-141">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-142">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-142">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0bad3-143">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="0bad3-143">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0bad3-144">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0bad3-144">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0bad3-145">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="0bad3-145">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0bad3-146">Remarques</span><span class="sxs-lookup"><span data-stu-id="0bad3-146">Remarks</span></span>

<span data-ttu-id="0bad3-p103">Impossible d'obtenir **ToRecipients** à l'aide d'une demande FindItem. Utiliser une demande de GetItem pour obtenir le **ToRecipients**.</span><span class="sxs-lookup"><span data-stu-id="0bad3-p103">You cannot get **ToRecipients** by using a FindItem request. Use a GetItem request to get the **ToRecipients**.</span></span>
  
<span data-ttu-id="0bad3-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0bad3-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bad3-150">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0bad3-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bad3-151">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0bad3-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bad3-152">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0bad3-152">Schema Name</span></span>  <br/> |<span data-ttu-id="0bad3-153">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0bad3-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bad3-154">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0bad3-154">Validation File</span></span>  <br/> |<span data-ttu-id="0bad3-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bad3-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bad3-156">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0bad3-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bad3-157">False</span><span class="sxs-lookup"><span data-stu-id="0bad3-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bad3-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0bad3-158">See also</span></span>



- [<span data-ttu-id="0bad3-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0bad3-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

