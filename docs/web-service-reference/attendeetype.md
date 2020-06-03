---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: L’élément AttendeeType représente le type de participant identifié dans l’élément email (EmailAddressType). Cet élément est utilisé dans les demandes de suggestions de réunion.
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462296"
---
# <a name="attendeetype"></a><span data-ttu-id="33246-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="33246-104">AttendeeType</span></span>

<span data-ttu-id="33246-105">L’élément **AttendeeType** représente le type de participant identifié dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="33246-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="33246-106">Cet élément est utilisé dans les demandes de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="33246-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="33246-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="33246-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="33246-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="33246-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="33246-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="33246-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="33246-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="33246-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="33246-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="33246-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33246-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="33246-112">Attributes and elements</span></span>

<span data-ttu-id="33246-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="33246-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33246-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="33246-114">Attributes</span></span>

<span data-ttu-id="33246-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="33246-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33246-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="33246-116">Child elements</span></span>

<span data-ttu-id="33246-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="33246-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33246-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="33246-118">Parent elements</span></span>

|<span data-ttu-id="33246-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="33246-119">**Element**</span></span>|<span data-ttu-id="33246-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="33246-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33246-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="33246-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="33246-122">Représente un utilisateur et des options de boîte aux lettres individuelle pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="33246-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="33246-123">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="33246-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33246-124">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="33246-124">Text value</span></span>

<span data-ttu-id="33246-125">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="33246-125">A text value is required for this element.</span></span> <span data-ttu-id="33246-126">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="33246-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="33246-127">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="33246-127">**Value**</span></span>|<span data-ttu-id="33246-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="33246-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33246-129">Organisateur</span><span class="sxs-lookup"><span data-stu-id="33246-129">Organizer</span></span>  <br/> |<span data-ttu-id="33246-130">Utilisateur de boîte aux lettres et participant qui a créé l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="33246-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="33246-131">Requis</span><span class="sxs-lookup"><span data-stu-id="33246-131">Required</span></span>  <br/> |<span data-ttu-id="33246-132">Utilisateur de boîte aux lettres qui est un participant obligatoire de la réunion.</span><span class="sxs-lookup"><span data-stu-id="33246-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="33246-133">Facultatif</span><span class="sxs-lookup"><span data-stu-id="33246-133">Optional</span></span>  <br/> |<span data-ttu-id="33246-134">Utilisateur de boîte aux lettres qui est un participant facultatif à la réunion.</span><span class="sxs-lookup"><span data-stu-id="33246-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="33246-135">Salle</span><span class="sxs-lookup"><span data-stu-id="33246-135">Room</span></span>  <br/> |<span data-ttu-id="33246-136">Entité de boîte aux lettres qui représente une ressource de salle utilisée pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="33246-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="33246-137">Resource</span><span class="sxs-lookup"><span data-stu-id="33246-137">Resource</span></span>  <br/> |<span data-ttu-id="33246-138">Ressource telle qu’un téléviseur ou un projecteur prévu pour être utilisée lors de la réunion.</span><span class="sxs-lookup"><span data-stu-id="33246-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33246-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="33246-139">Remarks</span></span>

<span data-ttu-id="33246-140">Cet élément est un élément enfant obligatoire de l’élément [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="33246-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="33246-141">Cet élément ne peut se produire qu’une seule fois dans l’élément [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="33246-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="33246-142">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="33246-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="33246-143">Le type de schéma AttendeeType est utilisé pour représenter les participants à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="33246-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="33246-144">Ne confondez pas cet élément avec des éléments du type de schéma AttendeeType.</span><span class="sxs-lookup"><span data-stu-id="33246-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="33246-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="33246-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33246-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="33246-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33246-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="33246-147">Schema Name</span></span>  <br/> |<span data-ttu-id="33246-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="33246-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="33246-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="33246-149">Validation File</span></span>  <br/> |<span data-ttu-id="33246-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="33246-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33246-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="33246-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="33246-152">False</span><span class="sxs-lookup"><span data-stu-id="33246-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33246-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="33246-153">See also</span></span>

- [<span data-ttu-id="33246-154">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="33246-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="33246-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="33246-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="33246-156">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="33246-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

