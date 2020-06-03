---
title: Option
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: L’élément item représente un élément générique dans la Banque d’Exchange.
ms.openlocfilehash: 72d8b1344bea3bcd105a0e293365b17f37193ac3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460315"
---
# <a name="item"></a><span data-ttu-id="c5680-103">Option</span><span class="sxs-lookup"><span data-stu-id="c5680-103">Item</span></span>

<span data-ttu-id="c5680-104">L’élément **Item** représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-104">The **Item** element represents a generic item in the Exchange store.</span></span> 
  
```xml
<Item>
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
</Item>
```

 <span data-ttu-id="c5680-105">**ItemType**</span><span class="sxs-lookup"><span data-stu-id="c5680-105">**ItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5680-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c5680-106">Attributes and elements</span></span>

<span data-ttu-id="c5680-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c5680-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5680-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c5680-108">Attributes</span></span>

<span data-ttu-id="c5680-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c5680-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5680-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c5680-110">Child elements</span></span>

|<span data-ttu-id="c5680-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5680-111">**Element**</span></span>|<span data-ttu-id="c5680-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5680-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5680-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="c5680-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="c5680-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="c5680-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="c5680-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="c5680-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c5680-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="c5680-117">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c5680-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c5680-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c5680-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="c5680-119">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="c5680-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="c5680-120">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c5680-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c5680-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="c5680-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="c5680-122">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="c5680-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="c5680-123">Objet</span><span class="sxs-lookup"><span data-stu-id="c5680-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="c5680-124">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="c5680-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="c5680-125">L’objet est limité à 255 caractères.</span><span class="sxs-lookup"><span data-stu-id="c5680-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="c5680-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="c5680-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="c5680-127">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="c5680-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="c5680-128">Body</span><span class="sxs-lookup"><span data-stu-id="c5680-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="c5680-129">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="c5680-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="c5680-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="c5680-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c5680-131">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c5680-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="c5680-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="c5680-133">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="c5680-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="c5680-134">Taille</span><span class="sxs-lookup"><span data-stu-id="c5680-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="c5680-p104">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c5680-p104">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c5680-137">Categories</span><span class="sxs-lookup"><span data-stu-id="c5680-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c5680-138">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="c5680-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="c5680-139">Importance</span><span class="sxs-lookup"><span data-stu-id="c5680-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="c5680-140">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="c5680-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="c5680-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="c5680-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="c5680-142">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="c5680-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="c5680-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="c5680-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="c5680-144">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="c5680-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="c5680-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="c5680-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="c5680-146">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="c5680-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="c5680-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="c5680-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="c5680-148">Indique si un utilisateur a envoyé un élément à lui-même.</span><span class="sxs-lookup"><span data-stu-id="c5680-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="c5680-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="c5680-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="c5680-150">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="c5680-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="c5680-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="c5680-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="c5680-152">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="c5680-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="c5680-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="c5680-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="c5680-154">Représente la collection de tous les en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c5680-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c5680-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="c5680-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="c5680-156">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="c5680-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="c5680-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="c5680-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="c5680-158">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="c5680-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="c5680-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="c5680-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="c5680-160">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c5680-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="c5680-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="c5680-p105">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="c5680-p105">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="c5680-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="c5680-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="c5680-165">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c5680-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="c5680-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="c5680-167">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="c5680-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c5680-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="c5680-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="c5680-169">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone CC.</span><span class="sxs-lookup"><span data-stu-id="c5680-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="c5680-170">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="c5680-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c5680-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="c5680-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="c5680-172">Représente la chaîne d’affichage qui est utilisée pour le contenu de la zone à.</span><span class="sxs-lookup"><span data-stu-id="c5680-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="c5680-173">Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="c5680-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c5680-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c5680-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="c5680-175">Représente une propriété qui est définie sur **true** si un élément comporte des pièces jointes au moins une pièce jointe visible.</span><span class="sxs-lookup"><span data-stu-id="c5680-175">Represents a property that is set to **true** if an item has attachments at least one visible attachment.</span></span> <span data-ttu-id="c5680-176">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c5680-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c5680-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c5680-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="c5680-178">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="c5680-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="c5680-179">Culture</span><span class="sxs-lookup"><span data-stu-id="c5680-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="c5680-180">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c5680-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c5680-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c5680-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c5680-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c5680-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c5680-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="c5680-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="c5680-185">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="c5680-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="c5680-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c5680-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="c5680-187">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="c5680-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="c5680-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="c5680-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="c5680-189">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="c5680-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="c5680-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c5680-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="c5680-191">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c5680-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c5680-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c5680-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="c5680-193">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="c5680-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c5680-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="c5680-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="c5680-195">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="c5680-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="c5680-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="c5680-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="c5680-197">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="c5680-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5680-198">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c5680-198">Parent elements</span></span>

|<span data-ttu-id="c5680-199">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5680-199">**Element**</span></span>|<span data-ttu-id="c5680-200">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5680-200">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5680-201">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="c5680-201">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="c5680-202">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="c5680-202">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c5680-203">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="c5680-203">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="c5680-204">Identifie les données à ajouter à une propriété unique d’un élément ou d’un dossier lors d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c5680-204">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c5680-205">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="c5680-205">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="c5680-206">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="c5680-206">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c5680-207">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c5680-207">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="c5680-208">Identifie un élément unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="c5680-208">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c5680-209">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c5680-209">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c5680-210">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-210">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c5680-211">Items</span><span class="sxs-lookup"><span data-stu-id="c5680-211">Items</span></span>](items.md) <br/> |<span data-ttu-id="c5680-212">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="c5680-212">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="c5680-213">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="c5680-213">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="c5680-214">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="c5680-214">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="c5680-215">SetItemField</span><span class="sxs-lookup"><span data-stu-id="c5680-215">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="c5680-216">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c5680-216">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c5680-217">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c5680-217">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="c5680-218">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="c5680-218">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5680-219">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c5680-219">Text value</span></span>

<span data-ttu-id="c5680-220">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c5680-220">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5680-221">Remarques</span><span class="sxs-lookup"><span data-stu-id="c5680-221">Remarks</span></span>

<span data-ttu-id="c5680-222">Il est important de noter que **ItemType** est le type de base pour les [tâches](task.md), les [CalendarItem](calendaritem.md), les [contacts](contact.md), les [DistributionList](distributionlist.md)et les [messages](message-ex15websvcsotherref.md).</span><span class="sxs-lookup"><span data-stu-id="c5680-222">It is important to note that **ItemType** is the base type for [Task](task.md), [CalendarItem](calendaritem.md), [Contact](contact.md), [DistributionList](distributionlist.md), and [Message](message-ex15websvcsotherref.md).</span></span>
  
<span data-ttu-id="c5680-223">Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="c5680-223">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="c5680-224">Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments **message** .</span><span class="sxs-lookup"><span data-stu-id="c5680-224">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="c5680-225">Microsoft Exchange Server 2010 ne renvoie pas l’élément **élément** de base dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="c5680-225">Microsoft Exchange Server 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="c5680-226">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5680-226">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5680-227">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c5680-227">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5680-228">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c5680-228">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5680-229">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c5680-229">Schema Name</span></span>  <br/> |<span data-ttu-id="c5680-230">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c5680-230">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5680-231">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c5680-231">Validation File</span></span>  <br/> |<span data-ttu-id="c5680-232">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c5680-232">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5680-233">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c5680-233">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5680-234">False</span><span class="sxs-lookup"><span data-stu-id="c5680-234">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5680-235">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5680-235">See also</span></span>



- [<span data-ttu-id="c5680-236">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c5680-236">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="c5680-237">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c5680-237">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

