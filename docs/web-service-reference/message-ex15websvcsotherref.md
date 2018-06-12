---
title: Message
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 2400b33c-43b2-4fc2-b6fb-275a99e0e810
description: L’élément de Message représente un message électronique de Microsoft Exchange.
ms.openlocfilehash: 388b944cfa16899cb2376320882f5087396d7b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828474"
---
# <a name="message"></a><span data-ttu-id="6eebd-103">Message</span><span class="sxs-lookup"><span data-stu-id="6eebd-103">Message</span></span>

<span data-ttu-id="6eebd-104">L’élément de **Message** représente un message électronique de Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
```xml
<Message>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ReminderMessageData/>
</Message>
```

 <span data-ttu-id="6eebd-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="6eebd-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6eebd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6eebd-106">Attributes and elements</span></span>

<span data-ttu-id="6eebd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6eebd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6eebd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6eebd-108">Attributes</span></span>

<span data-ttu-id="6eebd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6eebd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6eebd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6eebd-110">Child elements</span></span>

|<span data-ttu-id="6eebd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6eebd-111">**Element**</span></span>|<span data-ttu-id="6eebd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6eebd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6eebd-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="6eebd-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6eebd-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="6eebd-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="6eebd-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6eebd-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="6eebd-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6eebd-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6eebd-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6eebd-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="6eebd-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="6eebd-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6eebd-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6eebd-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6eebd-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-123">Objet</span><span class="sxs-lookup"><span data-stu-id="6eebd-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6eebd-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="6eebd-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="6eebd-125">L’objet est limitée à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="6eebd-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6eebd-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6eebd-127">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-128">Corps</span><span class="sxs-lookup"><span data-stu-id="6eebd-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="6eebd-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="6eebd-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="6eebd-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6eebd-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6eebd-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6eebd-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="6eebd-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-134">Taille</span><span class="sxs-lookup"><span data-stu-id="6eebd-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="6eebd-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6eebd-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-137">Categories</span><span class="sxs-lookup"><span data-stu-id="6eebd-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6eebd-138">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="6eebd-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-139">Importance</span><span class="sxs-lookup"><span data-stu-id="6eebd-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6eebd-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="6eebd-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6eebd-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="6eebd-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="6eebd-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6eebd-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="6eebd-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="6eebd-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6eebd-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6eebd-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="6eebd-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6eebd-148">Indique si un utilisateur a envoyé un élément pour lui ou elle-même.</span><span class="sxs-lookup"><span data-stu-id="6eebd-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="6eebd-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6eebd-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6eebd-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="6eebd-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6eebd-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="6eebd-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6eebd-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6eebd-154">Représente la collection de tous les en-têtes de message Internet qui sont contenues dans un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6eebd-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="6eebd-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6eebd-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6eebd-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6eebd-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6eebd-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="6eebd-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6eebd-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6eebd-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="6eebd-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6eebd-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="6eebd-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="6eebd-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="6eebd-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6eebd-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6eebd-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6eebd-167">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="6eebd-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="6eebd-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6eebd-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la ligne CC.</span><span class="sxs-lookup"><span data-stu-id="6eebd-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="6eebd-170">Il s’agit de la chaîne concaténée de tous les noms d’affichage du destinataire CC.</span><span class="sxs-lookup"><span data-stu-id="6eebd-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="6eebd-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6eebd-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="6eebd-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="6eebd-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="6eebd-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6eebd-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6eebd-p108">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="6eebd-p108">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="6eebd-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6eebd-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6eebd-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="6eebd-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-179">Culture</span><span class="sxs-lookup"><span data-stu-id="6eebd-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6eebd-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6eebd-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-181">Sender</span><span class="sxs-lookup"><span data-stu-id="6eebd-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="6eebd-182">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6eebd-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6eebd-184">Contient un ensemble de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="6eebd-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6eebd-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6eebd-186">Représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="6eebd-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6eebd-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6eebd-188">Représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="6eebd-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6eebd-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6eebd-190">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="6eebd-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6eebd-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6eebd-192">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="6eebd-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="6eebd-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="6eebd-194">Contient un ID binaire qui représente le thread auquel appartient ce message.</span><span class="sxs-lookup"><span data-stu-id="6eebd-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="6eebd-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="6eebd-196">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="6eebd-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-197">From</span><span class="sxs-lookup"><span data-stu-id="6eebd-197">From</span></span>](from.md) <br/> |<span data-ttu-id="6eebd-198">Représente le destinataire à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6eebd-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="6eebd-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="6eebd-200">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-201">Estlu</span><span class="sxs-lookup"><span data-stu-id="6eebd-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="6eebd-202">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="6eebd-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="6eebd-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="6eebd-204">Indique si une réponse à un message électronique est demandée.</span><span class="sxs-lookup"><span data-stu-id="6eebd-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-205">References</span><span class="sxs-lookup"><span data-stu-id="6eebd-205">References</span></span>](references.md) <br/> |<span data-ttu-id="6eebd-206">Représente l’en-tête Usenet qui est utilisé pour faire correspondre des réponses à leurs messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="6eebd-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="6eebd-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="6eebd-208">Identifie un ensemble d’adresses à laquelle les réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="6eebd-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-209">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="6eebd-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6eebd-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6eebd-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-212">Reçu par</span><span class="sxs-lookup"><span data-stu-id="6eebd-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6eebd-213">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6eebd-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-214">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6eebd-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6eebd-215">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6eebd-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-216">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="6eebd-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="6eebd-217">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="6eebd-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-218">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="6eebd-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="6eebd-219">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="6eebd-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-220">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="6eebd-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="6eebd-221">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="6eebd-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-222">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="6eebd-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="6eebd-223">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6eebd-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-224">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="6eebd-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="6eebd-225">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6eebd-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="6eebd-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="6eebd-227">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="6eebd-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="6eebd-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="6eebd-229">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="6eebd-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-230">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="6eebd-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="6eebd-231">Contient les données pour un message de rappel.</span><span class="sxs-lookup"><span data-stu-id="6eebd-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6eebd-232">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6eebd-232">Parent elements</span></span>

|<span data-ttu-id="6eebd-233">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6eebd-233">**Element**</span></span>|<span data-ttu-id="6eebd-234">**Description**</span><span class="sxs-lookup"><span data-stu-id="6eebd-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6eebd-235">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="6eebd-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6eebd-236">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6eebd-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-237">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="6eebd-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="6eebd-238">Identifie les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6eebd-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6eebd-239">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="6eebd-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6eebd-240">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6eebd-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-241">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="6eebd-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="6eebd-242">Identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="6eebd-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="6eebd-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="6eebd-244">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-245">Items</span><span class="sxs-lookup"><span data-stu-id="6eebd-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="6eebd-246">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="6eebd-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-247">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="6eebd-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6eebd-248">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="6eebd-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6eebd-249">SetItemField</span><span class="sxs-lookup"><span data-stu-id="6eebd-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="6eebd-250">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6eebd-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6eebd-251">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="6eebd-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="6eebd-252">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="6eebd-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6eebd-253">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6eebd-253">Text value</span></span>

<span data-ttu-id="6eebd-254">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6eebd-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6eebd-255">Remarques</span><span class="sxs-lookup"><span data-stu-id="6eebd-255">Remarks</span></span>

<span data-ttu-id="6eebd-256">Un autre élément de **Message** , [le Message (disponibilité)](message-availability.md) est utilisé par les opérations de disponibilité à renvoient des messages d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="6eebd-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="6eebd-257">Éléments de [message](message-ex15websvcsotherref.md) représentent des messages électroniques et tous les autres éléments qui ne sont pas fortement typées dans le schéma Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="6eebd-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="6eebd-258">Éléments tels que IPM. Partage et IPM.InfoPath sont renvoyés en tant qu’éléments du **Message** .</span><span class="sxs-lookup"><span data-stu-id="6eebd-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="6eebd-259">Exchange 2010 ne renvoie pas de **l’élément de base** des réponses.</span><span class="sxs-lookup"><span data-stu-id="6eebd-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="6eebd-260">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6eebd-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6eebd-261">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6eebd-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6eebd-262">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6eebd-262">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6eebd-263">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6eebd-263">Schema Name</span></span>  <br/> |<span data-ttu-id="6eebd-264">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6eebd-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="6eebd-265">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6eebd-265">Validation File</span></span>  <br/> |<span data-ttu-id="6eebd-266">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6eebd-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6eebd-267">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6eebd-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="6eebd-268">False</span><span class="sxs-lookup"><span data-stu-id="6eebd-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6eebd-269">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6eebd-269">See also</span></span>



- [<span data-ttu-id="6eebd-270">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6eebd-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

