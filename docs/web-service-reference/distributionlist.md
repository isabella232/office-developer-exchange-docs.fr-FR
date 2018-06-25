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
ms.openlocfilehash: 5edcc83eef6a5b16470e6c290aacd057ceecceb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756019"
---
# <a name="distributionlist"></a><span data-ttu-id="6e9ca-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="6e9ca-103">DistributionList</span></span>

<span data-ttu-id="6e9ca-104">L’élément **DistributionList** représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-104">The **DistributionList** element represents a distribution list.</span></span> 
  
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

 <span data-ttu-id="6e9ca-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="6e9ca-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e9ca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e9ca-106">Attributes and elements</span></span>

<span data-ttu-id="6e9ca-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e9ca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e9ca-108">Attributes</span></span>

<span data-ttu-id="6e9ca-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e9ca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e9ca-110">Child elements</span></span>

|<span data-ttu-id="6e9ca-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e9ca-111">**Element**</span></span>|<span data-ttu-id="6e9ca-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e9ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9ca-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="6e9ca-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6e9ca-114">Contient le flux MIME natif d’un objet représenté dans le format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="6e9ca-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6e9ca-116">Contient la clé unique identificateur et modification d’un élément de liste de distribution dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6e9ca-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6e9ca-118">Représente l’identificateur du dossier parent qui contient l’élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6e9ca-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6e9ca-120">Représente la classe de message d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-121">Objet</span><span class="sxs-lookup"><span data-stu-id="6e9ca-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6e9ca-122">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6e9ca-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6e9ca-124">Contient l’état de la sensibilité d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-125">Corps</span><span class="sxs-lookup"><span data-stu-id="6e9ca-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="6e9ca-126">Représente le contenu du corps d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-127">Pièces jointes</span><span class="sxs-lookup"><span data-stu-id="6e9ca-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6e9ca-128">Contient les éléments ou les fichiers associés à un élément de liste de distribution dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6e9ca-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6e9ca-130">Représente la date et l’heure à laquelle un élément de liste de distribution dans une boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-131">Size</span><span class="sxs-lookup"><span data-stu-id="6e9ca-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="6e9ca-132">Représente la taille, en octets, d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="6e9ca-133">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-134">Categories</span><span class="sxs-lookup"><span data-stu-id="6e9ca-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6e9ca-135">Représente une collection de chaînes qui identifient les catégories appartient un élément de liste de distribution dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-136">Importance</span><span class="sxs-lookup"><span data-stu-id="6e9ca-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6e9ca-137">Décrit l’importance d’un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="6e9ca-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6e9ca-139">Représente l’identificateur de l’élément de cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="6e9ca-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6e9ca-141">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="6e9ca-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6e9ca-143">Indique si un élément n'a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="6e9ca-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6e9ca-145">Indique si un utilisateur a envoyé un élément à lui-même.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="6e9ca-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6e9ca-147">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="6e9ca-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6e9ca-149">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6e9ca-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6e9ca-151">Représente la collection de tous les en-têtes de message Internet contenues dans un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="6e9ca-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6e9ca-153">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6e9ca-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6e9ca-155">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6e9ca-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6e9ca-157">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="6e9ca-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6e9ca-p102">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="6e9ca-p102">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="6e9ca-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="6e9ca-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6e9ca-162">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6e9ca-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6e9ca-164">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="6e9ca-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6e9ca-p103">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-p103">Represents the display string that is used for the contents of the Cc line. This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="6e9ca-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6e9ca-p104">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-p104">Represents the display string that is used for the contents of the To line. This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6e9ca-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6e9ca-p105">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="6e9ca-p105">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="6e9ca-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6e9ca-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6e9ca-175">Identifie les propriétés étendues sur un élément de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-176">Culture</span><span class="sxs-lookup"><span data-stu-id="6e9ca-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6e9ca-177">Représente la culture pour un élément de liste de distribution dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="6e9ca-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6e9ca-p106">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-p106">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="6e9ca-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="6e9ca-182">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-183">Heure de dernière modification</span><span class="sxs-lookup"><span data-stu-id="6e9ca-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="6e9ca-184">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="6e9ca-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="6e9ca-186">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="6e9ca-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="6e9ca-188">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="6e9ca-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="6e9ca-190">Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="6e9ca-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="6e9ca-192">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="6e9ca-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="6e9ca-194">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-195">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="6e9ca-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="6e9ca-196">Définit le nom complet d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-197">Classer sous</span><span class="sxs-lookup"><span data-stu-id="6e9ca-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="6e9ca-198">Représente la façon dont une liste de distribution est présentée dans le dossier Contacts.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="6e9ca-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="6e9ca-200">Indique si le contact se trouve dans la banque Exchange ou dans les Services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="6e9ca-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-201">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="6e9ca-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="6e9ca-202">Contient une liste des membres de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e9ca-203">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e9ca-203">Parent elements</span></span>

|<span data-ttu-id="6e9ca-204">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6e9ca-204">**Element**</span></span>|<span data-ttu-id="6e9ca-205">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e9ca-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9ca-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="6e9ca-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6e9ca-207">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="6e9ca-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="6e9ca-209">Identifie les données à ajouter à une propriété d’une liste de distribution pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6e9ca-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="6e9ca-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6e9ca-211">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-212">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="6e9ca-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="6e9ca-213">Identifie une liste de distribution à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-214">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="6e9ca-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="6e9ca-215">Identifie une liste de distribution pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-216">Items</span><span class="sxs-lookup"><span data-stu-id="6e9ca-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="6e9ca-217">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-218">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="6e9ca-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6e9ca-219">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6e9ca-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6e9ca-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="6e9ca-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="6e9ca-221">Représente une mise à jour d’une propriété d’un élément de liste de distribution dans une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6e9ca-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e9ca-222">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6e9ca-222">Text value</span></span>

<span data-ttu-id="6e9ca-223">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e9ca-224">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e9ca-224">Remarks</span></span>

<span data-ttu-id="6e9ca-225">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9ca-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e9ca-226">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e9ca-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e9ca-227">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e9ca-227">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e9ca-228">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e9ca-228">Schema Name</span></span>  <br/> |<span data-ttu-id="6e9ca-229">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6e9ca-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e9ca-230">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e9ca-230">Validation File</span></span>  <br/> |<span data-ttu-id="6e9ca-231">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e9ca-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e9ca-232">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e9ca-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e9ca-233">False</span><span class="sxs-lookup"><span data-stu-id="6e9ca-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e9ca-234">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e9ca-234">See also</span></span>

- [<span data-ttu-id="6e9ca-235">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6e9ca-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

