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
description: L’élément AttendeeType représente le type de participant est identifié dans l’élément de courrier électronique (EmailAddressType). Cet élément est utilisé dans les requêtes de suggestions de réunion.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755346"
---
# <a name="attendeetype"></a><span data-ttu-id="ee416-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="ee416-104">AttendeeType</span></span>

<span data-ttu-id="ee416-105">L’élément **AttendeeType** représente le type de participant est identifié dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="ee416-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="ee416-106">Cet élément est utilisé dans les requêtes de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="ee416-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="ee416-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ee416-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="ee416-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="ee416-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="ee416-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="ee416-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="ee416-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="ee416-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="ee416-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="ee416-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee416-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ee416-112">Attributes and elements</span></span>

<span data-ttu-id="ee416-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ee416-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee416-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="ee416-114">Attributes</span></span>

<span data-ttu-id="ee416-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ee416-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee416-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ee416-116">Child elements</span></span>

<span data-ttu-id="ee416-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ee416-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee416-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ee416-118">Parent elements</span></span>

|<span data-ttu-id="ee416-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ee416-119">**Element**</span></span>|<span data-ttu-id="ee416-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee416-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee416-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="ee416-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="ee416-122">Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ee416-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="ee416-123">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ee416-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee416-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ee416-124">Text value</span></span>

<span data-ttu-id="ee416-125">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="ee416-125">A text value is required for this element.</span></span> <span data-ttu-id="ee416-126">Le tableau suivant répertorie les valeurs possibles de cet élément.</span><span class="sxs-lookup"><span data-stu-id="ee416-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="ee416-127">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ee416-127">**Value**</span></span>|<span data-ttu-id="ee416-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee416-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee416-129">Organisateur</span><span class="sxs-lookup"><span data-stu-id="ee416-129">Organizer</span></span>  <br/> |<span data-ttu-id="ee416-130">L’utilisateur de boîte aux lettres et les participants qui a créé l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ee416-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="ee416-131">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="ee416-131">Required</span></span>  <br/> |<span data-ttu-id="ee416-132">Un utilisateur de boîte aux lettres qui est un participant obligatoire à la réunion.</span><span class="sxs-lookup"><span data-stu-id="ee416-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="ee416-133">Facultatif</span><span class="sxs-lookup"><span data-stu-id="ee416-133">Optional</span></span>  <br/> |<span data-ttu-id="ee416-134">Un utilisateur de boîte aux lettres qui est un participant facultatif à la réunion.</span><span class="sxs-lookup"><span data-stu-id="ee416-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="ee416-135">Salle</span><span class="sxs-lookup"><span data-stu-id="ee416-135">Room</span></span>  <br/> |<span data-ttu-id="ee416-136">Une entité de boîte aux lettres qui représente une ressource de l’espace utilisée pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="ee416-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="ee416-137">Ressource</span><span class="sxs-lookup"><span data-stu-id="ee416-137">Resource</span></span>  <br/> |<span data-ttu-id="ee416-138">Une ressource comme une télévision ou un projecteur qui est prévue pour une utilisation dans la réunion.</span><span class="sxs-lookup"><span data-stu-id="ee416-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee416-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="ee416-139">Remarks</span></span>

<span data-ttu-id="ee416-140">Cet élément est un élément enfant requis de l’élément [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="ee416-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="ee416-141">Cet élément ne peut apparaître qu’une seule fois dans l’élément [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="ee416-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="ee416-142">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ee416-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ee416-143">Le type de schéma AttendeeType est utilisé pour représenter les participants à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ee416-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="ee416-144">Ne confondez pas cet élément avec des éléments du type de schéma AttendeeType.</span><span class="sxs-lookup"><span data-stu-id="ee416-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ee416-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ee416-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee416-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ee416-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee416-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ee416-147">Schema Name</span></span>  <br/> |<span data-ttu-id="ee416-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ee416-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee416-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ee416-149">Validation File</span></span>  <br/> |<span data-ttu-id="ee416-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ee416-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee416-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ee416-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee416-152">False</span><span class="sxs-lookup"><span data-stu-id="ee416-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee416-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ee416-153">See also</span></span>

- [<span data-ttu-id="ee416-154">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ee416-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="ee416-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ee416-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="ee416-156">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="ee416-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

