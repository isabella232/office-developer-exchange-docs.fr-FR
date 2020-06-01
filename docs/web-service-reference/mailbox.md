---
title: Boîte aux lettres
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: L’élément Mailbox identifie un objet Active Directory à extension messagerie.
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468200"
---
# <a name="mailbox"></a><span data-ttu-id="ad95c-103">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ad95c-103">Mailbox</span></span>

<span data-ttu-id="ad95c-104">L’élément **Mailbox** identifie un objet Active Directory à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="ad95c-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="ad95c-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ad95c-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ad95c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad95c-106">Attributes and elements</span></span>

<span data-ttu-id="ad95c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad95c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad95c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad95c-108">Attributes</span></span>

<span data-ttu-id="ad95c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad95c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad95c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad95c-110">Child elements</span></span>

|<span data-ttu-id="ad95c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad95c-111">**Element**</span></span>|<span data-ttu-id="ad95c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad95c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad95c-113">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ad95c-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="ad95c-114">Définit le nom de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="ad95c-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad95c-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ad95c-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ad95c-117">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="ad95c-118">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad95c-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ad95c-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ad95c-120">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="ad95c-121">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="ad95c-121">The default is SMTP.</span></span> <span data-ttu-id="ad95c-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad95c-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ad95c-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ad95c-124">Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="ad95c-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad95c-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="ad95c-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ad95c-127">Définit l’identificateur d’élément d’une liste de distribution privée ou de contact pour les destinataires à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ad95c-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="ad95c-128">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ad95c-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad95c-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad95c-129">Parent elements</span></span>

|<span data-ttu-id="ad95c-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad95c-130">**Element**</span></span>|<span data-ttu-id="ad95c-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad95c-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad95c-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="ad95c-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="ad95c-133">Définit une demande de développement d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ad95c-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="ad95c-134">Voici l’expression XPath de cet élément :` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="ad95c-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="ad95c-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ad95c-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="ad95c-136">Contient un tableau de destinataires d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ad95c-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="ad95c-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="ad95c-138">Représente une collection de destinataires qui recevront une copie du message.</span><span class="sxs-lookup"><span data-stu-id="ad95c-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ad95c-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="ad95c-140">Représente une collection de destinataires qui reçoit une copie carbone invisible (CCI) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="ad95c-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="ad95c-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="ad95c-142">Identifie un tableau des adresses de messagerie auxquelles les réponses doivent être envoyées.</span><span class="sxs-lookup"><span data-stu-id="ad95c-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-143">Sender</span><span class="sxs-lookup"><span data-stu-id="ad95c-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="ad95c-144">Identifie l’expéditeur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="ad95c-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-145">From</span><span class="sxs-lookup"><span data-stu-id="ad95c-145">From</span></span>](from.md) <br/> |<span data-ttu-id="ad95c-146">Représente le destinataire à partir duquel le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="ad95c-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="ad95c-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="ad95c-148">Représente l’organisateur d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="ad95c-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ad95c-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="ad95c-150">Identifie les dossiers Microsoft Exchange Server 2007 par défaut.</span><span class="sxs-lookup"><span data-stu-id="ad95c-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="ad95c-151">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ad95c-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="ad95c-152">Solution</span><span class="sxs-lookup"><span data-stu-id="ad95c-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="ad95c-153">Contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="ad95c-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-154">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="ad95c-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="ad95c-155">Contient un tableau de boîtes aux lettres contenues dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ad95c-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-156">Participant</span><span class="sxs-lookup"><span data-stu-id="ad95c-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="ad95c-157">Représente les participants et les ressources d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ad95c-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="ad95c-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="ad95c-159">Définit une demande d’ajout de dossiers gérés à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="ad95c-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="ad95c-161">Définit une demande d’ajout de délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="ad95c-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="ad95c-163">Définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="ad95c-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="ad95c-165">Définit une demande de suppression de délégués d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="ad95c-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="ad95c-167">Définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad95c-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-168">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="ad95c-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="ad95c-169">Décrit le délégué dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ad95c-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ad95c-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="ad95c-171">Décrit le principal dans un scénario d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ad95c-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="ad95c-172">Membre</span><span class="sxs-lookup"><span data-stu-id="ad95c-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ad95c-173">Représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ad95c-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad95c-174">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad95c-174">Text value</span></span>

<span data-ttu-id="ad95c-175">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad95c-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad95c-176">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad95c-176">Remarks</span></span>

<span data-ttu-id="ad95c-177">Les éléments [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) et [ItemId](itemid.md) identifient une boîte aux lettres ou une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ad95c-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="ad95c-178">L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifie une boîte aux lettres ou une liste de distribution par adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="ad95c-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="ad95c-179">L’élément [ItemId](itemid.md) identifie une boîte aux lettres par un identificateur d’élément, qui est associé à une boîte aux lettres particulière.</span><span class="sxs-lookup"><span data-stu-id="ad95c-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="ad95c-180">L’élément [ItemId](itemid.md) ne peut pas être utilisé pour envoyer un message à une liste de distribution ou à un contact dans un dossier de contacts public.</span><span class="sxs-lookup"><span data-stu-id="ad95c-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="ad95c-181">Une erreur est générée si elle est utilisée dans une opération CreateItem, UpdateItem ou SendItem lorsqu’une tentative d’envoi d’un message à une liste de distribution ou à un contact dans un dossier public contacts est effectuée.</span><span class="sxs-lookup"><span data-stu-id="ad95c-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="ad95c-182">Utilisez l’opération ExpandDL pour obtenir l’adresse SMTP, puis envoyez le message à l’aide de l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) au lieu de l’élément [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="ad95c-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="ad95c-183">Un autre élément, [Mailbox (Availability)](mailbox-availability.md), fournit des informations pour les opérations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ad95c-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="ad95c-184">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad95c-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad95c-185">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad95c-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad95c-186">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad95c-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad95c-187">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad95c-187">Schema Name</span></span>  <br/> |<span data-ttu-id="ad95c-188">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ad95c-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad95c-189">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad95c-189">Validation File</span></span>  <br/> |<span data-ttu-id="ad95c-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad95c-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad95c-191">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad95c-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad95c-192">False</span><span class="sxs-lookup"><span data-stu-id="ad95c-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad95c-193">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad95c-193">See also</span></span>

- [<span data-ttu-id="ad95c-194">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad95c-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

