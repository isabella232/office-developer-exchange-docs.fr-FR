---
title: MeetingCancellation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingCancellation
api_type:
- schema
ms.assetid: a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea
description: L’élément MeetingCancellation représente une annulation de réunion dans la banque d’informations Exchange.
ms.openlocfilehash: b68135e2743c675bed92c54172369c2ef21f1a6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828447"
---
# <a name="meetingcancellation"></a><span data-ttu-id="ca83f-103">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ca83f-103">MeetingCancellation</span></span>

<span data-ttu-id="ca83f-104">L’élément **MeetingCancellation** représente une annulation de réunion dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
```xml
<MeetingCancellation>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
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
</MeetingCancellation>
```

 <span data-ttu-id="ca83f-105">**MeetingCancellationMessageType**</span><span class="sxs-lookup"><span data-stu-id="ca83f-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca83f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca83f-106">Attributes and elements</span></span>

<span data-ttu-id="ca83f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca83f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca83f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca83f-108">Attributes</span></span>

<span data-ttu-id="ca83f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca83f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca83f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca83f-110">Child elements</span></span>

|<span data-ttu-id="ca83f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca83f-111">**Element**</span></span>|<span data-ttu-id="ca83f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca83f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca83f-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="ca83f-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="ca83f-114">Contient le flux MIME natif d’un objet qui est représenté dans le format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="ca83f-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ca83f-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ca83f-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="ca83f-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ca83f-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ca83f-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ca83f-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ca83f-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="ca83f-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ca83f-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ca83f-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ca83f-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-123">Objet</span><span class="sxs-lookup"><span data-stu-id="ca83f-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="ca83f-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="ca83f-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="ca83f-125">L’objet est limitée à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="ca83f-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ca83f-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="ca83f-127">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-128">Corps</span><span class="sxs-lookup"><span data-stu-id="ca83f-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="ca83f-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="ca83f-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="ca83f-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ca83f-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ca83f-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="ca83f-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="ca83f-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-134">Taille</span><span class="sxs-lookup"><span data-stu-id="ca83f-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="ca83f-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ca83f-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-137">Categories</span><span class="sxs-lookup"><span data-stu-id="ca83f-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ca83f-138">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="ca83f-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-139">Importance</span><span class="sxs-lookup"><span data-stu-id="ca83f-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="ca83f-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="ca83f-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="ca83f-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="ca83f-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ca83f-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="ca83f-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="ca83f-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ca83f-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="ca83f-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ca83f-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ca83f-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="ca83f-148">Indique si un utilisateur a envoyé un élément pour lui ou elle-même.</span><span class="sxs-lookup"><span data-stu-id="ca83f-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="ca83f-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="ca83f-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ca83f-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ca83f-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="ca83f-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="ca83f-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ca83f-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="ca83f-154">Représente la collection de tous les en-têtes de message Internet qui sont contenues dans un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ca83f-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ca83f-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="ca83f-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ca83f-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ca83f-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="ca83f-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="ca83f-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ca83f-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ca83f-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="ca83f-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="ca83f-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="ca83f-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="ca83f-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="ca83f-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="ca83f-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ca83f-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="ca83f-167">Représente le nombre de minutes avant un événement d’affichage d’un rappel.</span><span class="sxs-lookup"><span data-stu-id="ca83f-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="ca83f-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="ca83f-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone Cc.</span><span class="sxs-lookup"><span data-stu-id="ca83f-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="ca83f-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="ca83f-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="ca83f-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="ca83f-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="ca83f-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="ca83f-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="ca83f-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ca83f-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="ca83f-p108">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="ca83f-p108">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="ca83f-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ca83f-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ca83f-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="ca83f-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-179">Culture</span><span class="sxs-lookup"><span data-stu-id="ca83f-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="ca83f-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ca83f-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ca83f-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ca83f-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ca83f-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="ca83f-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="ca83f-185">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-186">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="ca83f-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ca83f-187">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="ca83f-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="ca83f-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="ca83f-189">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="ca83f-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ca83f-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="ca83f-191">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ca83f-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ca83f-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="ca83f-193">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ca83f-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="ca83f-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="ca83f-195">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="ca83f-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="ca83f-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="ca83f-197">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="ca83f-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-198">Sender</span><span class="sxs-lookup"><span data-stu-id="ca83f-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="ca83f-199">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ca83f-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="ca83f-201">Contient un ensemble de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="ca83f-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="ca83f-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="ca83f-203">Représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="ca83f-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ca83f-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="ca83f-205">Représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="ca83f-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-206">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ca83f-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="ca83f-207">Indique si l’expéditeur d’un élément demande une confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="ca83f-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-208">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ca83f-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="ca83f-209">Indique si l’expéditeur d’un élément demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="ca83f-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="ca83f-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="ca83f-211">Contient un ID binaire qui représente le thread auquel appartient ce message.</span><span class="sxs-lookup"><span data-stu-id="ca83f-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="ca83f-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="ca83f-213">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="ca83f-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-214">From</span><span class="sxs-lookup"><span data-stu-id="ca83f-214">From</span></span>](from.md) <br/> |<span data-ttu-id="ca83f-215">Représente le destinataire à partir de laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ca83f-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="ca83f-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="ca83f-217">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ca83f-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-218">Estlu</span><span class="sxs-lookup"><span data-stu-id="ca83f-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="ca83f-219">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="ca83f-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-220">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="ca83f-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="ca83f-221">Indique si une réponse à un message électronique est demandée.</span><span class="sxs-lookup"><span data-stu-id="ca83f-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-222">References</span><span class="sxs-lookup"><span data-stu-id="ca83f-222">References</span></span>](references.md) <br/> |<span data-ttu-id="ca83f-223">Représente l’en-tête Usenet qui est utilisé pour faire correspondre des réponses à leurs messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="ca83f-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="ca83f-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="ca83f-225">Identifie un ensemble d’adresses à laquelle les réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="ca83f-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-226">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="ca83f-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="ca83f-227">Représente l’élément de calendrier qui est associé à un [MeetingMessage](meetingmessage.md).</span><span class="sxs-lookup"><span data-stu-id="ca83f-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="ca83f-228">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="ca83f-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="ca83f-229">Indique si une réunion a été gérée par un compte avec l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ca83f-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="ca83f-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="ca83f-231">Indique si un message de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="ca83f-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-232">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="ca83f-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="ca83f-233">Indique si un message de réunion élément a été traité.</span><span class="sxs-lookup"><span data-stu-id="ca83f-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="ca83f-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="ca83f-235">Représente le type de destinataire réponse reçue pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="ca83f-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-236">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ca83f-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ca83f-237">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="ca83f-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ca83f-238">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="ca83f-238">This element is read-only.</span></span> <span data-ttu-id="ca83f-239">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ca83f-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ca83f-240">Reçu par</span><span class="sxs-lookup"><span data-stu-id="ca83f-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="ca83f-241">Identifie le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ca83f-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="ca83f-242">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ca83f-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-243">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ca83f-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="ca83f-244">Identifie le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ca83f-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="ca83f-245">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ca83f-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-246">UID</span><span class="sxs-lookup"><span data-stu-id="ca83f-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="ca83f-247">Identifie un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ca83f-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-248">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="ca83f-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="ca83f-249">Utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca83f-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-250">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="ca83f-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="ca83f-251">Indique la date et l’heure de création d’une instance d’un objet iCalendar.</span><span class="sxs-lookup"><span data-stu-id="ca83f-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca83f-252">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca83f-252">Parent elements</span></span>

|<span data-ttu-id="ca83f-253">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca83f-253">**Element**</span></span>|<span data-ttu-id="ca83f-254">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca83f-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca83f-255">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ca83f-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="ca83f-256">Identifie tous les éléments de calendrier sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="ca83f-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-257">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ca83f-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ca83f-258">Identifie les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ca83f-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ca83f-259">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ca83f-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="ca83f-260">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="ca83f-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-261">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ca83f-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ca83f-262">Identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="ca83f-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-263">Items</span><span class="sxs-lookup"><span data-stu-id="ca83f-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="ca83f-264">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="ca83f-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-265">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="ca83f-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="ca83f-266">Contient un tableau d’éléments à créer.</span><span class="sxs-lookup"><span data-stu-id="ca83f-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ca83f-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ca83f-268">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="ca83f-269">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ca83f-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ca83f-270">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ca83f-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ca83f-271">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ca83f-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ca83f-272">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="ca83f-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca83f-273">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ca83f-273">Text value</span></span>

<span data-ttu-id="ca83f-274">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca83f-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca83f-275">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca83f-275">Remarks</span></span>

<span data-ttu-id="ca83f-276">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca83f-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca83f-277">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ca83f-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca83f-278">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ca83f-278">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca83f-279">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ca83f-279">Schema Name</span></span>  <br/> |<span data-ttu-id="ca83f-280">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ca83f-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca83f-281">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ca83f-281">Validation File</span></span>  <br/> |<span data-ttu-id="ca83f-282">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ca83f-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca83f-283">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ca83f-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca83f-284">False</span><span class="sxs-lookup"><span data-stu-id="ca83f-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca83f-285">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca83f-285">See also</span></span>



- [<span data-ttu-id="ca83f-286">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ca83f-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

