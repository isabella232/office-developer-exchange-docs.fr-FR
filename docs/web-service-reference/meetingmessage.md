---
title: MeetingMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingMessage
api_type:
- schema
ms.assetid: c95956a8-7505-44b4-bea4-11d1f5182796
description: L’élément MeetingMessage représente une réunion dans la Banque d’aide Exchange.
ms.openlocfilehash: fee615a1da117e5df03cd5ce8576bd66d7e89a4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468382"
---
# <a name="meetingmessage"></a><span data-ttu-id="00e75-103">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="00e75-103">MeetingMessage</span></span>

<span data-ttu-id="00e75-104">L’élément **MeetingMessage** représente une réunion dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-104">The **MeetingMessage** element represents a meeting in the Exchange store.</span></span> 
  
```xml
<MeetingMessage>
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
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</MeetingMessage>
```

 <span data-ttu-id="00e75-105">**MeetingMessageType**</span><span class="sxs-lookup"><span data-stu-id="00e75-105">**MeetingMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00e75-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00e75-106">Attributes and elements</span></span>

<span data-ttu-id="00e75-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00e75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00e75-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00e75-108">Attributes</span></span>

<span data-ttu-id="00e75-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00e75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00e75-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00e75-110">Child elements</span></span>

|<span data-ttu-id="00e75-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00e75-111">**Element**</span></span>|<span data-ttu-id="00e75-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00e75-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00e75-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="00e75-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="00e75-114">Contient le flux MIME natif d’un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="00e75-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="00e75-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="00e75-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="00e75-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="00e75-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="00e75-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="00e75-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="00e75-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="00e75-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="00e75-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="00e75-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="00e75-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="00e75-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="00e75-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="00e75-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-123">Objet</span><span class="sxs-lookup"><span data-stu-id="00e75-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="00e75-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="00e75-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="00e75-125">L’objet est limité à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="00e75-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="00e75-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="00e75-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="00e75-127">Contient l’état du critère de diffusion d’un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-127">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="00e75-128">Body</span><span class="sxs-lookup"><span data-stu-id="00e75-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="00e75-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="00e75-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="00e75-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="00e75-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="00e75-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="00e75-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="00e75-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="00e75-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="00e75-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="00e75-134">Taille</span><span class="sxs-lookup"><span data-stu-id="00e75-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="00e75-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="00e75-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="00e75-137">Categories</span><span class="sxs-lookup"><span data-stu-id="00e75-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="00e75-138">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="00e75-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="00e75-139">Importance</span><span class="sxs-lookup"><span data-stu-id="00e75-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="00e75-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="00e75-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="00e75-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="00e75-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="00e75-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="00e75-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="00e75-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="00e75-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="00e75-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="00e75-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="00e75-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="00e75-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="00e75-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="00e75-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="00e75-148">Indique si un utilisateur s’est envoyé un élément à lui-même ou à lui-même.</span><span class="sxs-lookup"><span data-stu-id="00e75-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="00e75-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="00e75-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="00e75-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="00e75-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="00e75-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="00e75-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="00e75-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="00e75-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="00e75-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="00e75-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="00e75-154">Représente la collection de tous les en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="00e75-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="00e75-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="00e75-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="00e75-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="00e75-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="00e75-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="00e75-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="00e75-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="00e75-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="00e75-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="00e75-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="00e75-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="00e75-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="00e75-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="00e75-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="00e75-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="00e75-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="00e75-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="00e75-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="00e75-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="00e75-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="00e75-167">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="00e75-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="00e75-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="00e75-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="00e75-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone CC.</span><span class="sxs-lookup"><span data-stu-id="00e75-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="00e75-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="00e75-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="00e75-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="00e75-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="00e75-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="00e75-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="00e75-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="00e75-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="00e75-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="00e75-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="00e75-175">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible.</span><span class="sxs-lookup"><span data-stu-id="00e75-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="00e75-176">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="00e75-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="00e75-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="00e75-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="00e75-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="00e75-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="00e75-179">Culture</span><span class="sxs-lookup"><span data-stu-id="00e75-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="00e75-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="00e75-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="00e75-181">Sender</span><span class="sxs-lookup"><span data-stu-id="00e75-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="00e75-182">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="00e75-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="00e75-184">Contient un ensemble de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="00e75-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="00e75-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="00e75-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="00e75-186">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="00e75-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="00e75-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="00e75-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="00e75-188">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="00e75-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="00e75-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="00e75-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="00e75-190">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="00e75-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="00e75-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="00e75-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="00e75-192">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="00e75-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="00e75-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="00e75-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="00e75-194">Contient un ID binaire qui représente le thread auquel ce message appartient.</span><span class="sxs-lookup"><span data-stu-id="00e75-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="00e75-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="00e75-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="00e75-196">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="00e75-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="00e75-197">From</span><span class="sxs-lookup"><span data-stu-id="00e75-197">From</span></span>](from.md) <br/> |<span data-ttu-id="00e75-198">Représente le destinataire à partir duquel le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="00e75-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="00e75-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="00e75-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="00e75-200">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="00e75-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="00e75-202">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="00e75-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="00e75-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="00e75-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="00e75-204">Indique si une réponse à un message électronique est demandée.</span><span class="sxs-lookup"><span data-stu-id="00e75-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="00e75-205">References</span><span class="sxs-lookup"><span data-stu-id="00e75-205">References</span></span>](references.md) <br/> |<span data-ttu-id="00e75-206">Représente l’en-tête Usenet qui est utilisé pour corréler les réponses avec leurs messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="00e75-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="00e75-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="00e75-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="00e75-208">Identifie un ensemble d’adresses auxquelles des réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="00e75-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="00e75-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="00e75-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="00e75-210">Représente l’élément de calendrier associé à un [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="00e75-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="00e75-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="00e75-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="00e75-212">Indique si une réunion a été gérée par un compte disposant d’un accès délégué.</span><span class="sxs-lookup"><span data-stu-id="00e75-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="00e75-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="00e75-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="00e75-214">Indique si un message de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="00e75-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="00e75-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="00e75-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="00e75-216">Indique si un élément de message de réunion a été traité.</span><span class="sxs-lookup"><span data-stu-id="00e75-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="00e75-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="00e75-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="00e75-218">Représente le type de réponse de destinataire reçue pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="00e75-218">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="00e75-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="00e75-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="00e75-220">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="00e75-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="00e75-221">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="00e75-221">This element is read-only.</span></span> <span data-ttu-id="00e75-222">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="00e75-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="00e75-223">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="00e75-223">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="00e75-224">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="00e75-224">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-225">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="00e75-225">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="00e75-226">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="00e75-226">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="00e75-227">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="00e75-227">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="00e75-228">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="00e75-228">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="00e75-229">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="00e75-229">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="00e75-230">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="00e75-230">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="00e75-231">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="00e75-231">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="00e75-232">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="00e75-232">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="00e75-233">ConversationId</span><span class="sxs-lookup"><span data-stu-id="00e75-233">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="00e75-234">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="00e75-234">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="00e75-235">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="00e75-235">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="00e75-236">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="00e75-236">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="00e75-237">UID</span><span class="sxs-lookup"><span data-stu-id="00e75-237">UID</span></span>](uid.md) <br/> |<span data-ttu-id="00e75-238">Identifie un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="00e75-238">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-239">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="00e75-239">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="00e75-240">Permet d’identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="00e75-240">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="00e75-241">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="00e75-241">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="00e75-242">Indique la date et l’heure de création d’une instance d’un objet iCalendar.</span><span class="sxs-lookup"><span data-stu-id="00e75-242">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00e75-243">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00e75-243">Parent elements</span></span>

|<span data-ttu-id="00e75-244">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00e75-244">**Element**</span></span>|<span data-ttu-id="00e75-245">**Description**</span><span class="sxs-lookup"><span data-stu-id="00e75-245">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00e75-246">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="00e75-246">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="00e75-247">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="00e75-247">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="00e75-248">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="00e75-248">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="00e75-249">Identifie les données à ajouter à une propriété unique d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="00e75-249">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="00e75-250">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="00e75-250">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="00e75-251">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="00e75-251">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="00e75-252">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="00e75-252">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="00e75-253">Identifie un élément unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="00e75-253">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="00e75-254">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="00e75-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="00e75-255">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="00e75-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="00e75-256">Items</span><span class="sxs-lookup"><span data-stu-id="00e75-256">Items</span></span>](items.md) <br/> |<span data-ttu-id="00e75-257">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="00e75-257">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="00e75-258">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="00e75-258">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="00e75-259">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="00e75-259">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="00e75-260">SetItemField</span><span class="sxs-lookup"><span data-stu-id="00e75-260">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="00e75-261">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="00e75-261">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="00e75-262">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="00e75-262">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="00e75-263">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-263">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00e75-264">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="00e75-264">Text value</span></span>

<span data-ttu-id="00e75-265">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00e75-265">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00e75-266">Remarques</span><span class="sxs-lookup"><span data-stu-id="00e75-266">Remarks</span></span>

<span data-ttu-id="00e75-267">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00e75-267">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00e75-268">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00e75-268">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00e75-269">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00e75-269">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00e75-270">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00e75-270">Schema Name</span></span>  <br/> |<span data-ttu-id="00e75-271">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="00e75-271">Types schema</span></span>  <br/> |
|<span data-ttu-id="00e75-272">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00e75-272">Validation File</span></span>  <br/> |<span data-ttu-id="00e75-273">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00e75-273">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00e75-274">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00e75-274">Can be Empty</span></span>  <br/> |<span data-ttu-id="00e75-275">False</span><span class="sxs-lookup"><span data-stu-id="00e75-275">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00e75-276">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00e75-276">See also</span></span>



- [<span data-ttu-id="00e75-277">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00e75-277">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

