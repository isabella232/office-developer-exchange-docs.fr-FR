---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: L’élément DistributionList représente une liste de distribution.
ms.openlocfilehash: 5eb97bef349ca02848f65fa58370b9c81c6653d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457003"
---
# <a name="distributionlist"></a><span data-ttu-id="0ee14-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0ee14-103">DistributionList</span></span>

<span data-ttu-id="0ee14-104">L’élément **DistributionList** représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-104">The **DistributionList** element represents a distribution list.</span></span> 
  
```xml
<DistributionList>
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
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 <span data-ttu-id="0ee14-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="0ee14-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ee14-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ee14-106">Attributes and elements</span></span>

<span data-ttu-id="0ee14-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ee14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ee14-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ee14-108">Attributes</span></span>

<span data-ttu-id="0ee14-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0ee14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ee14-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ee14-110">Child elements</span></span>

|<span data-ttu-id="0ee14-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ee14-111">**Element**</span></span>|<span data-ttu-id="0ee14-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ee14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ee14-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="0ee14-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="0ee14-114">Contient le flux MIME natif d’un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="0ee14-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="0ee14-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0ee14-116">Contient l’identificateur unique et la clé de modification d’un élément de liste de distribution dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ee14-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0ee14-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0ee14-118">Représente l’identificateur du dossier parent qui contient l’élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0ee14-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="0ee14-120">Représente la classe de message d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-121">Objet</span><span class="sxs-lookup"><span data-stu-id="0ee14-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="0ee14-122">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="0ee14-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0ee14-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="0ee14-124">Contient l’état du critère de diffusion d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-125">Corps</span><span class="sxs-lookup"><span data-stu-id="0ee14-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="0ee14-126">Représente le contenu réel du corps d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="0ee14-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ee14-128">Contient les éléments ou les fichiers joints à un élément de liste de distribution dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ee14-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0ee14-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="0ee14-130">Représente la date et l’heure auxquelles un élément de liste de distribution d’une boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="0ee14-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-131">Taille</span><span class="sxs-lookup"><span data-stu-id="0ee14-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="0ee14-132">Représente la taille, en octets, d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="0ee14-133">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ee14-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-134">Categories</span><span class="sxs-lookup"><span data-stu-id="0ee14-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ee14-135">Représente une collection de chaînes qui identifient les catégories auxquelles un élément de liste de distribution appartient à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ee14-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-136">Importance</span><span class="sxs-lookup"><span data-stu-id="0ee14-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="0ee14-137">Décrit l’importance d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="0ee14-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="0ee14-139">Représente l’identificateur de l’élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="0ee14-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="0ee14-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="0ee14-141">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="0ee14-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="0ee14-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="0ee14-143">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ee14-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="0ee14-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="0ee14-145">Indique si un utilisateur a envoyé un élément à lui-même.</span><span class="sxs-lookup"><span data-stu-id="0ee14-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="0ee14-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="0ee14-147">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ee14-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="0ee14-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="0ee14-149">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="0ee14-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="0ee14-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="0ee14-151">Représente la collection de tous les en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ee14-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="0ee14-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="0ee14-153">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="0ee14-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0ee14-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="0ee14-155">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="0ee14-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0ee14-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0ee14-157">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ee14-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="0ee14-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="0ee14-p102">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="0ee14-p102">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="0ee14-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="0ee14-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="0ee14-162">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ee14-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0ee14-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="0ee14-164">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="0ee14-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="0ee14-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="0ee14-p103">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="0ee14-p103">Represents the display string that is used for the contents of the Cc line. This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="0ee14-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="0ee14-p104">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="0ee14-p104">Represents the display string that is used for the contents of the To line. This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0ee14-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="0ee14-p105">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="0ee14-p105">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="0ee14-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0ee14-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="0ee14-175">Identifie les propriétés étendues d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-176">Culture</span><span class="sxs-lookup"><span data-stu-id="0ee14-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="0ee14-177">Représente la culture d’un élément de liste de distribution dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ee14-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="0ee14-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0ee14-p106">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0ee14-p106">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="0ee14-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="0ee14-182">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="0ee14-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0ee14-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0ee14-184">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="0ee14-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="0ee14-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="0ee14-186">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="0ee14-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0ee14-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="0ee14-188">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0ee14-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="0ee14-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="0ee14-190">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0ee14-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="0ee14-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="0ee14-192">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="0ee14-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="0ee14-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="0ee14-194">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="0ee14-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-195">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="0ee14-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="0ee14-196">Définit le nom d’affichage d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="0ee14-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="0ee14-198">Représente l’archivage d’une liste de distribution dans le dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="0ee14-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="0ee14-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="0ee14-200">Indique si le contact se trouve dans la Banque d’information Exchange ou dans les services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0ee14-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="0ee14-201">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="0ee14-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="0ee14-202">Contient une liste des membres de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0ee14-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ee14-203">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ee14-203">Parent elements</span></span>

|<span data-ttu-id="0ee14-204">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ee14-204">**Element**</span></span>|<span data-ttu-id="0ee14-205">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ee14-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ee14-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="0ee14-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="0ee14-207">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="0ee14-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="0ee14-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="0ee14-209">Identifie les données à ajouter à une propriété unique d’une liste de distribution pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0ee14-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0ee14-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="0ee14-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="0ee14-211">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="0ee14-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-212">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0ee14-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="0ee14-213">Identifie une liste de distribution unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="0ee14-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-214">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0ee14-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="0ee14-215">Identifie une liste de distribution unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="0ee14-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-216">Items</span><span class="sxs-lookup"><span data-stu-id="0ee14-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="0ee14-217">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="0ee14-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-218">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="0ee14-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="0ee14-219">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="0ee14-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="0ee14-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="0ee14-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="0ee14-221">Représente une mise à jour d’une propriété unique d’un élément de liste de distribution dans une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0ee14-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ee14-222">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0ee14-222">Text value</span></span>

<span data-ttu-id="0ee14-223">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ee14-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ee14-224">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ee14-224">Remarks</span></span>

<span data-ttu-id="0ee14-225">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ee14-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ee14-226">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ee14-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ee14-227">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ee14-227">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ee14-228">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ee14-228">Schema Name</span></span>  <br/> |<span data-ttu-id="0ee14-229">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0ee14-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ee14-230">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ee14-230">Validation File</span></span>  <br/> |<span data-ttu-id="0ee14-231">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ee14-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ee14-232">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ee14-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ee14-233">False</span><span class="sxs-lookup"><span data-stu-id="0ee14-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ee14-234">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ee14-234">See also</span></span>

- [<span data-ttu-id="0ee14-235">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0ee14-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

