---
title: Objet postItem
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
description: L’élément PostItem représente un élément de publication dans la banque d’informations Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828866"
---
# <a name="postitem"></a><span data-ttu-id="1a745-103">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="1a745-103">PostItem</span></span>

<span data-ttu-id="1a745-104">L’élément **PostItem** représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="1a745-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="1a745-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a745-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a745-106">Attributes and elements</span></span>

<span data-ttu-id="1a745-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a745-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a745-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a745-108">Attributes</span></span>

<span data-ttu-id="1a745-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a745-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a745-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a745-110">Child elements</span></span>

|<span data-ttu-id="1a745-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a745-111">**Element**</span></span>|<span data-ttu-id="1a745-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a745-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a745-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="1a745-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="1a745-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="1a745-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="1a745-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="1a745-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1a745-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="1a745-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1a745-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1a745-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1a745-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="1a745-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="1a745-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1a745-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="1a745-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="1a745-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-123">Objet</span><span class="sxs-lookup"><span data-stu-id="1a745-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="1a745-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="1a745-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="1a745-125">L’objet est limitée à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="1a745-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="1a745-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="1a745-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="1a745-127">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-128">Corps</span><span class="sxs-lookup"><span data-stu-id="1a745-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="1a745-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="1a745-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="1a745-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="1a745-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1a745-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1a745-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="1a745-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="1a745-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="1a745-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="1a745-134">Taille</span><span class="sxs-lookup"><span data-stu-id="1a745-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="1a745-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1a745-137">Categories</span><span class="sxs-lookup"><span data-stu-id="1a745-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1a745-138">Représente une collection de chaînes qui identifient les catégories auquel appartient un élément dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a745-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="1a745-139">Importance</span><span class="sxs-lookup"><span data-stu-id="1a745-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="1a745-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="1a745-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="1a745-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="1a745-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="1a745-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="1a745-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="1a745-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="1a745-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="1a745-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="1a745-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="1a745-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="1a745-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="1a745-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="1a745-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="1a745-148">Indique si un utilisateur a envoyé un élément pour lui ou elle-même.</span><span class="sxs-lookup"><span data-stu-id="1a745-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="1a745-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="1a745-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="1a745-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="1a745-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="1a745-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="1a745-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="1a745-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="1a745-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="1a745-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="1a745-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="1a745-154">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a745-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1a745-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="1a745-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="1a745-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="1a745-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="1a745-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="1a745-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="1a745-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="1a745-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="1a745-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="1a745-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="1a745-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1a745-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="1a745-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="1a745-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="1a745-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="1a745-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="1a745-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="1a745-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1a745-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="1a745-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="1a745-167">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="1a745-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="1a745-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="1a745-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="1a745-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone Cc.</span><span class="sxs-lookup"><span data-stu-id="1a745-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="1a745-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="1a745-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1a745-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="1a745-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="1a745-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="1a745-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="1a745-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="1a745-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1a745-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="1a745-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="1a745-175">Représente une propriété qui est définie sur **true** si un élément a au moins une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="1a745-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="1a745-176">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1a745-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1a745-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="1a745-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="1a745-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="1a745-179">Culture</span><span class="sxs-lookup"><span data-stu-id="1a745-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="1a745-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a745-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1a745-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="1a745-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1a745-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1a745-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="1a745-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="1a745-185">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-186">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="1a745-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="1a745-187">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="1a745-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="1a745-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="1a745-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="1a745-189">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="1a745-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="1a745-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="1a745-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="1a745-191">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="1a745-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="1a745-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="1a745-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="1a745-193">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="1a745-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="1a745-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="1a745-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="1a745-195">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="1a745-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="1a745-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="1a745-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="1a745-197">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="1a745-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="1a745-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="1a745-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="1a745-199">Contient un ID binaire qui représente le thread auquel appartient ce message.</span><span class="sxs-lookup"><span data-stu-id="1a745-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="1a745-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="1a745-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="1a745-201">Représente l’identificateur de la conversation.</span><span class="sxs-lookup"><span data-stu-id="1a745-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="1a745-202">From</span><span class="sxs-lookup"><span data-stu-id="1a745-202">From</span></span>](from.md) <br/> |<span data-ttu-id="1a745-203">Représente l’adresse à partir de laquelle l’élément de message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="1a745-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="1a745-204">L’élément **à partir de** peut uniquement être définie au moment de la création.</span><span class="sxs-lookup"><span data-stu-id="1a745-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="1a745-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="1a745-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="1a745-206">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-207">Estlu</span><span class="sxs-lookup"><span data-stu-id="1a745-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="1a745-208">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="1a745-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="1a745-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="1a745-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="1a745-210">Représente l’heure à laquelle un [objet PostItem](postitem.md) a été validée.</span><span class="sxs-lookup"><span data-stu-id="1a745-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="1a745-211">References</span><span class="sxs-lookup"><span data-stu-id="1a745-211">References</span></span>](references.md) <br/> |<span data-ttu-id="1a745-212">Représente l’en-tête Usenet qui est utilisé pour associer des réponses avec les messages d’origine.</span><span class="sxs-lookup"><span data-stu-id="1a745-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="1a745-213">Sender</span><span class="sxs-lookup"><span data-stu-id="1a745-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="1a745-214">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="1a745-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a745-215">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a745-215">Parent elements</span></span>

|<span data-ttu-id="1a745-216">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a745-216">**Element**</span></span>|<span data-ttu-id="1a745-217">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a745-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a745-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="1a745-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="1a745-219">Représente une mise à jour d’une propriété unique d’un élément dans une opération UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="1a745-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="1a745-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="1a745-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="1a745-221">Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1a745-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1a745-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="1a745-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="1a745-223">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="1a745-224">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="1a745-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="1a745-225">Identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="1a745-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1a745-226">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="1a745-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="1a745-227">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="1a745-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1a745-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="1a745-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="1a745-229">Renvoyées dans les réponses [SyncFolderItems](syncfolderitems.md) lorsqu’un élément a été lu.</span><span class="sxs-lookup"><span data-stu-id="1a745-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="1a745-230">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="1a745-230">This property is read-only.</span></span> <span data-ttu-id="1a745-231">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1a745-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1a745-232">Items</span><span class="sxs-lookup"><span data-stu-id="1a745-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="1a745-233">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="1a745-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="1a745-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="1a745-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="1a745-235">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="1a745-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1a745-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="1a745-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="1a745-237">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="1a745-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a745-238">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1a745-238">Text value</span></span>

<span data-ttu-id="1a745-239">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a745-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a745-240">Remarques</span><span class="sxs-lookup"><span data-stu-id="1a745-240">Remarks</span></span>

<span data-ttu-id="1a745-241">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a745-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a745-242">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1a745-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a745-243">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1a745-243">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a745-244">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1a745-244">Schema Name</span></span>  <br/> |<span data-ttu-id="1a745-245">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1a745-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a745-246">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1a745-246">Validation File</span></span>  <br/> |<span data-ttu-id="1a745-247">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a745-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a745-248">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1a745-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a745-249">False</span><span class="sxs-lookup"><span data-stu-id="1a745-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a745-250">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a745-250">See also</span></span>



- [<span data-ttu-id="1a745-251">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a745-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

