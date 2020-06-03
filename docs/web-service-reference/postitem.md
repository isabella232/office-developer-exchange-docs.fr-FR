---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: L’élément PostItem représente un élément post dans la Banque d’Exchange.
ms.openlocfilehash: 5fba1a9a6a3abc95ea2ce65cafa2b62bc7423f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528866"
---
# <a name="postitem"></a><span data-ttu-id="0ec93-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="0ec93-103">PostItem</span></span>

<span data-ttu-id="0ec93-104">L’élément **PostItem** représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
```xml
<PostItem>
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
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 <span data-ttu-id="0ec93-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="0ec93-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ec93-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ec93-106">Attributes and elements</span></span>

<span data-ttu-id="0ec93-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ec93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ec93-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ec93-108">Attributes</span></span>

<span data-ttu-id="0ec93-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0ec93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ec93-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ec93-110">Child elements</span></span>

|<span data-ttu-id="0ec93-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ec93-111">**Element**</span></span>|<span data-ttu-id="0ec93-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ec93-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ec93-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="0ec93-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="0ec93-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="0ec93-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="0ec93-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0ec93-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="0ec93-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0ec93-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0ec93-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="0ec93-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="0ec93-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0ec93-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="0ec93-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-123">Objet</span><span class="sxs-lookup"><span data-stu-id="0ec93-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="0ec93-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="0ec93-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="0ec93-125">L’objet est limité à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="0ec93-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0ec93-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="0ec93-127">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-128">Body</span><span class="sxs-lookup"><span data-stu-id="0ec93-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="0ec93-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="0ec93-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="0ec93-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ec93-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0ec93-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="0ec93-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="0ec93-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-134">Taille</span><span class="sxs-lookup"><span data-stu-id="0ec93-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="0ec93-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-137">Categories</span><span class="sxs-lookup"><span data-stu-id="0ec93-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ec93-138">Représente une collection de chaînes qui identifient les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="0ec93-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-139">Importance</span><span class="sxs-lookup"><span data-stu-id="0ec93-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="0ec93-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="0ec93-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="0ec93-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="0ec93-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="0ec93-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="0ec93-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="0ec93-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="0ec93-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="0ec93-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ec93-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="0ec93-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="0ec93-148">Indique si un utilisateur s’est envoyé un élément à lui-même ou à lui-même.</span><span class="sxs-lookup"><span data-stu-id="0ec93-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="0ec93-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="0ec93-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ec93-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="0ec93-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="0ec93-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="0ec93-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="0ec93-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="0ec93-154">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ec93-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="0ec93-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="0ec93-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ec93-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0ec93-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="0ec93-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="0ec93-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0ec93-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0ec93-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="0ec93-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="0ec93-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="0ec93-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="0ec93-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="0ec93-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="0ec93-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0ec93-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="0ec93-167">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="0ec93-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="0ec93-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="0ec93-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone CC.</span><span class="sxs-lookup"><span data-stu-id="0ec93-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="0ec93-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="0ec93-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="0ec93-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="0ec93-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="0ec93-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="0ec93-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="0ec93-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0ec93-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="0ec93-175">Représente une propriété qui est définie sur **true** si un élément a au moins une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="0ec93-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="0ec93-176">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0ec93-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="0ec93-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="0ec93-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-179">Culture</span><span class="sxs-lookup"><span data-stu-id="0ec93-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="0ec93-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ec93-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="0ec93-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0ec93-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="0ec93-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="0ec93-185">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0ec93-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0ec93-187">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="0ec93-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="0ec93-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="0ec93-189">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="0ec93-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0ec93-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="0ec93-191">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0ec93-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0ec93-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="0ec93-193">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0ec93-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="0ec93-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="0ec93-195">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="0ec93-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="0ec93-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="0ec93-197">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="0ec93-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="0ec93-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="0ec93-199">Contient un ID binaire qui représente le thread auquel ce message appartient.</span><span class="sxs-lookup"><span data-stu-id="0ec93-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="0ec93-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="0ec93-201">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="0ec93-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-202">From</span><span class="sxs-lookup"><span data-stu-id="0ec93-202">From</span></span>](from.md) <br/> |<span data-ttu-id="0ec93-203">Représente l’adresse à partir de laquelle l’élément a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ec93-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="0ec93-204">L’élément **from** ne peut être défini qu’au moment de la création.</span><span class="sxs-lookup"><span data-stu-id="0ec93-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="0ec93-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="0ec93-206">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="0ec93-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="0ec93-208">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="0ec93-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="0ec93-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="0ec93-210">Représente l’heure à laquelle un [PostItem](postitem.md) a été publié.</span><span class="sxs-lookup"><span data-stu-id="0ec93-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-211">References</span><span class="sxs-lookup"><span data-stu-id="0ec93-211">References</span></span>](references.md) <br/> |<span data-ttu-id="0ec93-212">Représente l’en-tête Usenet qui est utilisé pour associer les réponses aux messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="0ec93-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-213">Sender</span><span class="sxs-lookup"><span data-stu-id="0ec93-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="0ec93-214">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="0ec93-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ec93-215">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ec93-215">Parent elements</span></span>

|<span data-ttu-id="0ec93-216">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ec93-216">**Element**</span></span>|<span data-ttu-id="0ec93-217">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ec93-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ec93-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="0ec93-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="0ec93-219">Représente une mise à jour d'une propriété unique d'un élément dans une UpdateItem Operation.</span><span class="sxs-lookup"><span data-stu-id="0ec93-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="0ec93-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="0ec93-221">Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0ec93-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0ec93-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0ec93-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="0ec93-223">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-224">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0ec93-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="0ec93-225">Identifie un élément unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="0ec93-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-226">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0ec93-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="0ec93-227">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="0ec93-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="0ec93-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="0ec93-229">Renvoyée dans les réponses [SyncFolderItems](syncfolderitems.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="0ec93-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="0ec93-230">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ec93-230">This property is read-only.</span></span> <span data-ttu-id="0ec93-231">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0ec93-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-232">Items</span><span class="sxs-lookup"><span data-stu-id="0ec93-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="0ec93-233">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="0ec93-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="0ec93-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="0ec93-235">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="0ec93-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0ec93-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="0ec93-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="0ec93-237">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="0ec93-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ec93-238">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0ec93-238">Text value</span></span>

<span data-ttu-id="0ec93-239">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ec93-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ec93-240">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ec93-240">Remarks</span></span>

<span data-ttu-id="0ec93-241">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ec93-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ec93-242">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ec93-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ec93-243">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ec93-243">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ec93-244">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ec93-244">Schema Name</span></span>  <br/> |<span data-ttu-id="0ec93-245">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0ec93-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ec93-246">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ec93-246">Validation File</span></span>  <br/> |<span data-ttu-id="0ec93-247">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ec93-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ec93-248">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ec93-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ec93-249">False</span><span class="sxs-lookup"><span data-stu-id="0ec93-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ec93-250">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ec93-250">See also</span></span>



- [<span data-ttu-id="0ec93-251">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0ec93-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

