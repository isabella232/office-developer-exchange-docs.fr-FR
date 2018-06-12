---
title: Contact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: L'élément Contact représente un contact dans la banque d'informations Exchange.
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755557"
---
# <a name="contact"></a><span data-ttu-id="e832e-103">Contact</span><span class="sxs-lookup"><span data-stu-id="e832e-103">Contact</span></span>

<span data-ttu-id="e832e-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **Contact** représente un contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 <span data-ttu-id="e832e-105">**ContactItemType**</span><span class="sxs-lookup"><span data-stu-id="e832e-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e832e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e832e-106">Attributes and elements</span></span>

<span data-ttu-id="e832e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e832e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e832e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e832e-108">Attributes</span></span>

<span data-ttu-id="e832e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e832e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e832e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e832e-110">Child elements</span></span>

|<span data-ttu-id="e832e-111">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="e832e-111">**Element name**</span></span>|<span data-ttu-id="e832e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e832e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e832e-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="e832e-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="e832e-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="e832e-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="e832e-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="e832e-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e832e-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e832e-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e832e-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e832e-118">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="e832e-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="e832e-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e832e-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="e832e-120">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="e832e-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-121">Objet</span><span class="sxs-lookup"><span data-stu-id="e832e-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="e832e-122">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="e832e-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="e832e-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="e832e-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="e832e-124">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="e832e-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-125">Corps</span><span class="sxs-lookup"><span data-stu-id="e832e-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="e832e-126">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="e832e-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="e832e-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="e832e-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e832e-128">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e832e-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="e832e-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="e832e-130">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="e832e-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="e832e-131">Taille</span><span class="sxs-lookup"><span data-stu-id="e832e-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="e832e-p101">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e832e-p101">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e832e-134">Categories</span><span class="sxs-lookup"><span data-stu-id="e832e-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e832e-135">Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="e832e-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="e832e-136">Importance</span><span class="sxs-lookup"><span data-stu-id="e832e-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="e832e-137">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="e832e-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="e832e-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="e832e-139">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="e832e-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="e832e-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="e832e-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="e832e-141">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="e832e-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="e832e-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="e832e-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="e832e-143">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="e832e-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="e832e-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="e832e-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="e832e-145">Indique si un utilisateur s'est envoyé un élément à lui-même.</span><span class="sxs-lookup"><span data-stu-id="e832e-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="e832e-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="e832e-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="e832e-147">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="e832e-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="e832e-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="e832e-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="e832e-149">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="e832e-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="e832e-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="e832e-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="e832e-151">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e832e-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e832e-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="e832e-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="e832e-153">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="e832e-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="e832e-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="e832e-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="e832e-155">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="e832e-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="e832e-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e832e-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e832e-157">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e832e-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="e832e-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="e832e-p102">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="e832e-p102">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="e832e-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="e832e-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="e832e-162">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e832e-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="e832e-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="e832e-164">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="e832e-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="e832e-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="e832e-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="e832e-p103">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="e832e-p103">Represents the display string that is used for the contents of the Cc line. This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e832e-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="e832e-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="e832e-p104">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="e832e-p104">Represents the display string that is used for the contents of the To line. This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e832e-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="e832e-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="e832e-p105">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="e832e-p105">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="e832e-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e832e-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="e832e-175">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="e832e-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="e832e-176">Culture</span><span class="sxs-lookup"><span data-stu-id="e832e-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="e832e-177">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e832e-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e832e-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e832e-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e832e-p106">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e832e-p106">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e832e-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="e832e-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="e832e-182">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="e832e-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-183">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="e832e-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="e832e-184">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="e832e-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="e832e-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="e832e-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="e832e-186">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="e832e-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="e832e-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="e832e-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="e832e-188">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e832e-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="e832e-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="e832e-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="e832e-190">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e832e-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="e832e-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="e832e-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="e832e-192">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="e832e-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="e832e-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="e832e-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="e832e-194">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="e832e-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="e832e-195">Classer sous</span><span class="sxs-lookup"><span data-stu-id="e832e-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="e832e-196">Indique comment un contact est classé dans le dossier Contacts.</span><span class="sxs-lookup"><span data-stu-id="e832e-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e832e-197">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="e832e-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="e832e-198">Définit la construction de l'affichage d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-199">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e832e-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e832e-200">Définit le nom d'affichage d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-201">Prénom</span><span class="sxs-lookup"><span data-stu-id="e832e-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="e832e-202">Contient le nom d'un contact donné.</span><span class="sxs-lookup"><span data-stu-id="e832e-202">Contains a contact's given name.</span></span>  <br/> |
|[<span data-ttu-id="e832e-203">Initials</span><span class="sxs-lookup"><span data-stu-id="e832e-203">Initials</span></span>](initials.md) <br/> |<span data-ttu-id="e832e-204">Représente les initiales d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-205">MiddleName</span><span class="sxs-lookup"><span data-stu-id="e832e-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="e832e-206">Représente le deuxième prénom d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-207">Nickname</span><span class="sxs-lookup"><span data-stu-id="e832e-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="e832e-208">Représente le surnom d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-209">CompleteName</span><span class="sxs-lookup"><span data-stu-id="e832e-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="e832e-210">Représente le nom complet d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-210">Represents the complete name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-211">CompanyName</span><span class="sxs-lookup"><span data-stu-id="e832e-211">CompanyName</span></span>](companyname.md) <br/> |<span data-ttu-id="e832e-212">Représente le nom de la société associée à un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="e832e-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="e832e-214">Représente une collection d'adresses de messagerie pour un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-215">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="e832e-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="e832e-216">Contient une collection d'adresses physiques associées à un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="e832e-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="e832e-218">Représente une collection de numéros de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="e832e-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="e832e-220">Représente un assistant d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-221">Anniversaire</span><span class="sxs-lookup"><span data-stu-id="e832e-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="e832e-222">Représente la date de naissance d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="e832e-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="e832e-224">Représente la page d'accueil (adresse web) d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-225">Enfants</span><span class="sxs-lookup"><span data-stu-id="e832e-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="e832e-226">Contient les noms des enfants d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="e832e-227">Companies</span><span class="sxs-lookup"><span data-stu-id="e832e-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="e832e-228">Représente la collection de sociétés associées à un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-229">ContactSource</span><span class="sxs-lookup"><span data-stu-id="e832e-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="e832e-230">Indique si le contact se trouve dans la banque d'informations Exchange ou dans le service d'annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e832e-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="e832e-231">Department</span><span class="sxs-lookup"><span data-stu-id="e832e-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="e832e-232">Représente le service du contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="e832e-233">Génération</span><span class="sxs-lookup"><span data-stu-id="e832e-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="e832e-234">Représente une abréviation de génération suivant le nom complet d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-235">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="e832e-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="e832e-236">Représente une collection d'adresses de messagerie instantanée pour un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-237">JobTitle</span><span class="sxs-lookup"><span data-stu-id="e832e-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="e832e-238">Représente la fonction d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-239">Manager</span><span class="sxs-lookup"><span data-stu-id="e832e-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="e832e-240">Représente le responsable d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="e832e-241">Mileage</span><span class="sxs-lookup"><span data-stu-id="e832e-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="e832e-242">Représente le kilométrage d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-243">OfficeLocation</span><span class="sxs-lookup"><span data-stu-id="e832e-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="e832e-244">Représente l'emplacement du bureau d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-245">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="e832e-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="e832e-246">Représente les types d'affichage pour les adresses physiques.</span><span class="sxs-lookup"><span data-stu-id="e832e-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="e832e-247">Profession</span><span class="sxs-lookup"><span data-stu-id="e832e-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="e832e-248">Représente la profession d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-249">NomEpoux</span><span class="sxs-lookup"><span data-stu-id="e832e-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="e832e-250">Représente le nom du conjoint d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="e832e-251">Surname</span><span class="sxs-lookup"><span data-stu-id="e832e-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="e832e-252">Représente le nom de famille d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-253">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="e832e-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="e832e-254">Contient l'anniversaire de mariage d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="e832e-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="e832e-256">Indique si le contact comporte une photo du contact en pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="e832e-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="e832e-257">PhoneticFullName</span><span class="sxs-lookup"><span data-stu-id="e832e-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="e832e-258">Contient le nom complet d'un contact, y compris son prénom et son nom, orthographié phonétiquement.</span><span class="sxs-lookup"><span data-stu-id="e832e-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="e832e-259">PhoneticFirstName</span><span class="sxs-lookup"><span data-stu-id="e832e-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="e832e-260">Contient le prénom d'un contact, orthographié phonétiquement.</span><span class="sxs-lookup"><span data-stu-id="e832e-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="e832e-261">PhoneticLastName</span><span class="sxs-lookup"><span data-stu-id="e832e-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="e832e-262">Contient le nom d'un contact, orthographié phonétiquement.</span><span class="sxs-lookup"><span data-stu-id="e832e-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="e832e-263">Alias</span><span class="sxs-lookup"><span data-stu-id="e832e-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="e832e-264">Contient l'alias de messagerie d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-265">Notes (contacts)</span><span class="sxs-lookup"><span data-stu-id="e832e-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="e832e-266">Contient des informations supplémentaires sur le contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-266">Contains supplementary contact information.</span></span>  <br/> |
|[<span data-ttu-id="e832e-267">photo</span><span class="sxs-lookup"><span data-stu-id="e832e-267">Photo</span></span>](photo.md) <br/> |<span data-ttu-id="e832e-268">Contient une valeur qui code la photo d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="e832e-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="e832e-270">Contient une valeur qui code le certificat SMIME d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-271">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="e832e-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="e832e-272">Contient une valeur qui code le certificat Microsoft Exchange d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-273">DirectoryId</span><span class="sxs-lookup"><span data-stu-id="e832e-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="e832e-274">Contient l'identificateur du répertoire d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-275">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="e832e-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="e832e-276">Contient des informations SMTP qui identifient la boîte aux lettres du responsable du contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="e832e-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="e832e-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="e832e-278">Contient des informations SMTP qui identifient les collaborateurs directs d'un contact.</span><span class="sxs-lookup"><span data-stu-id="e832e-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e832e-279">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e832e-279">Parent elements</span></span>

|<span data-ttu-id="e832e-280">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="e832e-280">**Element name**</span></span>|<span data-ttu-id="e832e-281">**Description**</span><span class="sxs-lookup"><span data-stu-id="e832e-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e832e-282">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="e832e-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="e832e-283">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="e832e-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e832e-284">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="e832e-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="e832e-285">Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e832e-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e832e-286">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="e832e-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="e832e-287">Identifie tous les éléments qui entrent en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="e832e-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="e832e-288">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e832e-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="e832e-289">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="e832e-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e832e-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="e832e-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="e832e-291">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="e832e-292">Items</span><span class="sxs-lookup"><span data-stu-id="e832e-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="e832e-293">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="e832e-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="e832e-294">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e832e-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e832e-295">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="e832e-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e832e-296">Solution</span><span class="sxs-lookup"><span data-stu-id="e832e-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="e832e-297">Contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="e832e-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="e832e-298">SetItemField</span><span class="sxs-lookup"><span data-stu-id="e832e-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="e832e-299">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e832e-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e832e-300">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e832e-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="e832e-301">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="e832e-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e832e-302">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e832e-302">Text value</span></span>

<span data-ttu-id="e832e-303">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e832e-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e832e-304">Remarques</span><span class="sxs-lookup"><span data-stu-id="e832e-304">Remarks</span></span>

<span data-ttu-id="e832e-305">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e832e-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e832e-306">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e832e-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e832e-307">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e832e-307">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e832e-308">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e832e-308">Schema name</span></span>  <br/> |<span data-ttu-id="e832e-309">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e832e-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="e832e-310">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e832e-310">Validation file</span></span>  <br/> |<span data-ttu-id="e832e-311">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e832e-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e832e-312">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e832e-312">Can be empty</span></span>  <br/> |<span data-ttu-id="e832e-313">False</span><span class="sxs-lookup"><span data-stu-id="e832e-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e832e-314">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e832e-314">See also</span></span>



- [<span data-ttu-id="e832e-315">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e832e-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e832e-316">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="e832e-316">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="e832e-317">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="e832e-317">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="e832e-318">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="e832e-318">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

