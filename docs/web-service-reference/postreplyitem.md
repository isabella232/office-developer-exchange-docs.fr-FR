---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: L’élément PostReplyItem contient une réponse à un élément de publication. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 4104e79449acc6e358b729cf2de769d28dac52bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461680"
---
# <a name="postreplyitem"></a><span data-ttu-id="6dda3-104">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="6dda3-104">PostReplyItem</span></span>

<span data-ttu-id="6dda3-105">L’élément **PostReplyItem** contient une réponse à un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="6dda3-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="6dda3-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6dda3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostReplyItem>
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
   <NewBodyContent/>
</PostReplyItem>
```

 <span data-ttu-id="6dda3-107">**PostReplyItemType**</span><span class="sxs-lookup"><span data-stu-id="6dda3-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dda3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6dda3-108">Attributes and elements</span></span>

<span data-ttu-id="6dda3-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6dda3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dda3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6dda3-110">Attributes</span></span>

<span data-ttu-id="6dda3-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6dda3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6dda3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6dda3-112">Child elements</span></span>

|<span data-ttu-id="6dda3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6dda3-113">**Element**</span></span>|<span data-ttu-id="6dda3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6dda3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dda3-115">MimeContent</span><span class="sxs-lookup"><span data-stu-id="6dda3-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6dda3-116">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="6dda3-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="6dda3-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6dda3-118">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda3-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="6dda3-119">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6dda3-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6dda3-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6dda3-121">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="6dda3-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="6dda3-122">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6dda3-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6dda3-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6dda3-124">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6dda3-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-125">Objet</span><span class="sxs-lookup"><span data-stu-id="6dda3-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6dda3-126">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="6dda3-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="6dda3-127">L’objet est limité à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="6dda3-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6dda3-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6dda3-129">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6dda3-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-130">Body</span><span class="sxs-lookup"><span data-stu-id="6dda3-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="6dda3-131">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="6dda3-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-132">Attachments</span><span class="sxs-lookup"><span data-stu-id="6dda3-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6dda3-133">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda3-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6dda3-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6dda3-135">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="6dda3-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-136">Taille</span><span class="sxs-lookup"><span data-stu-id="6dda3-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="6dda3-p106">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6dda3-p106">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-139">Categories</span><span class="sxs-lookup"><span data-stu-id="6dda3-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6dda3-140">Représente une collection de chaînes qui identifient les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="6dda3-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-141">Importance</span><span class="sxs-lookup"><span data-stu-id="6dda3-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6dda3-142">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6dda3-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-143">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="6dda3-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6dda3-144">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="6dda3-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-145">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="6dda3-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6dda3-146">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="6dda3-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="6dda3-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6dda3-148">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-149">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="6dda3-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6dda3-150">Indique si un utilisateur s’est envoyé un élément à lui-même ou à lui-même.</span><span class="sxs-lookup"><span data-stu-id="6dda3-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-151">IsResend</span><span class="sxs-lookup"><span data-stu-id="6dda3-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6dda3-152">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-153">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="6dda3-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6dda3-154">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="6dda3-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6dda3-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6dda3-156">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6dda3-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-157">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="6dda3-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6dda3-158">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6dda3-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6dda3-160">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-161">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6dda3-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6dda3-162">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda3-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-163">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="6dda3-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6dda3-p107">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="6dda3-p107">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="6dda3-166">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="6dda3-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6dda3-167">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda3-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6dda3-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6dda3-169">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="6dda3-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-170">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="6dda3-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6dda3-p108">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="6dda3-p108">Represents the display string that is used for the contents of the Cc line. This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-173">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="6dda3-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6dda3-174">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="6dda3-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="6dda3-175">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="6dda3-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6dda3-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6dda3-177">Représente une propriété qui est définie sur **true** si un élément a une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="6dda3-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="6dda3-178">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6dda3-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6dda3-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6dda3-180">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="6dda3-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-181">Culture</span><span class="sxs-lookup"><span data-stu-id="6dda3-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6dda3-182">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6dda3-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-183">Sender</span><span class="sxs-lookup"><span data-stu-id="6dda3-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="6dda3-184">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="6dda3-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6dda3-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6dda3-186">Contient un ensemble de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="6dda3-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6dda3-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6dda3-188">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="6dda3-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6dda3-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6dda3-190">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="6dda3-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-191">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6dda3-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6dda3-192">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="6dda3-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-193">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6dda3-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6dda3-194">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="6dda3-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="6dda3-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="6dda3-196">Contient un ID binaire qui représente le thread auquel ce message appartient.</span><span class="sxs-lookup"><span data-stu-id="6dda3-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="6dda3-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="6dda3-198">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="6dda3-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-199">From</span><span class="sxs-lookup"><span data-stu-id="6dda3-199">From</span></span>](from.md) <br/> |<span data-ttu-id="6dda3-200">Représente l’adresse à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="6dda3-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="6dda3-202">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="6dda3-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="6dda3-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="6dda3-204">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="6dda3-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-205">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="6dda3-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="6dda3-206">Indique si une réponse à un message électronique est demandée.</span><span class="sxs-lookup"><span data-stu-id="6dda3-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-207">References</span><span class="sxs-lookup"><span data-stu-id="6dda3-207">References</span></span>](references.md) <br/> |<span data-ttu-id="6dda3-208">Représente l’en-tête Usenet qui est utilisé pour associer les réponses à leurs messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="6dda3-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="6dda3-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="6dda3-210">Identifie un ensemble d’adresses auxquelles des réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="6dda3-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-211">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="6dda3-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6dda3-212">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="6dda3-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="6dda3-213">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6dda3-213">This element is read-only.</span></span> <span data-ttu-id="6dda3-214">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6dda3-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-215">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="6dda3-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6dda3-216">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6dda3-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="6dda3-217">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6dda3-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-218">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6dda3-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6dda3-219">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="6dda3-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="6dda3-220">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6dda3-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-221">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="6dda3-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="6dda3-222">Représente le nouveau corps de texte d’un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="6dda3-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6dda3-223">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6dda3-223">Parent elements</span></span>

|<span data-ttu-id="6dda3-224">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6dda3-224">**Element**</span></span>|<span data-ttu-id="6dda3-225">**Description**</span><span class="sxs-lookup"><span data-stu-id="6dda3-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dda3-226">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="6dda3-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6dda3-227">Décrit tous les éléments adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6dda3-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-228">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="6dda3-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6dda3-229">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6dda3-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-230">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6dda3-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6dda3-231">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda3-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda3-232">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="6dda3-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6dda3-233">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="6dda3-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6dda3-234">Remarques</span><span class="sxs-lookup"><span data-stu-id="6dda3-234">Remarks</span></span>

<span data-ttu-id="6dda3-235">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6dda3-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dda3-236">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6dda3-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dda3-237">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6dda3-237">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6dda3-238">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6dda3-238">Schema Name</span></span>  <br/> |<span data-ttu-id="6dda3-239">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6dda3-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="6dda3-240">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6dda3-240">Validation File</span></span>  <br/> |<span data-ttu-id="6dda3-241">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6dda3-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6dda3-242">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6dda3-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="6dda3-243">False</span><span class="sxs-lookup"><span data-stu-id="6dda3-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6dda3-244">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6dda3-244">See also</span></span>



- [<span data-ttu-id="6dda3-245">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6dda3-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

