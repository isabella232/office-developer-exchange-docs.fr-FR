---
title: CalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: L’élément CalendarItem représente un élément de calendrier Exchange.
ms.openlocfilehash: b29141470d157ef5bd67be06a1e1fa1c9536b042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529482"
---
# <a name="calendaritem"></a><span data-ttu-id="37768-103">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="37768-103">CalendarItem</span></span>

<span data-ttu-id="37768-104">L’élément **CalendarItem** représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-104">The **CalendarItem** element represents an Exchange calendar item.</span></span> 
  
```XML
<CalendarItem>
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
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 <span data-ttu-id="37768-105">**CalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="37768-105">**CalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37768-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37768-106">Attributes and elements</span></span>

<span data-ttu-id="37768-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37768-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37768-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37768-108">Attributes</span></span>

<span data-ttu-id="37768-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="37768-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37768-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37768-110">Child elements</span></span>

|<span data-ttu-id="37768-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37768-111">**Element**</span></span>|<span data-ttu-id="37768-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="37768-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37768-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="37768-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="37768-114">Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.</span><span class="sxs-lookup"><span data-stu-id="37768-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="37768-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="37768-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="37768-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37768-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="37768-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="37768-118">Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="37768-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="37768-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="37768-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="37768-120">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="37768-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="37768-121">Objet</span><span class="sxs-lookup"><span data-stu-id="37768-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="37768-122">Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="37768-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="37768-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="37768-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="37768-124">Indique le niveau de confidentialité d'un élément.</span><span class="sxs-lookup"><span data-stu-id="37768-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="37768-125">Body</span><span class="sxs-lookup"><span data-stu-id="37768-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="37768-126">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="37768-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="37768-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="37768-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="37768-128">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37768-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="37768-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="37768-130">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.</span><span class="sxs-lookup"><span data-stu-id="37768-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="37768-131">Taille</span><span class="sxs-lookup"><span data-stu-id="37768-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="37768-p101">Représente la taille en octets d'un élément. Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="37768-p101">Represents the size in bytes of an item. This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="37768-134">Categories</span><span class="sxs-lookup"><span data-stu-id="37768-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="37768-135">Représente une collection de chaînes qui identifient les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="37768-135">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="37768-136">Importance</span><span class="sxs-lookup"><span data-stu-id="37768-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="37768-137">Décrit l'importance d'un élément.</span><span class="sxs-lookup"><span data-stu-id="37768-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="37768-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="37768-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="37768-139">Représente l'identificateur de l'élément dont cet élément est une réponse.</span><span class="sxs-lookup"><span data-stu-id="37768-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="37768-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="37768-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="37768-141">Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.</span><span class="sxs-lookup"><span data-stu-id="37768-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="37768-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="37768-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="37768-143">Indique si un élément n’a pas encore été envoyé.</span><span class="sxs-lookup"><span data-stu-id="37768-143">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="37768-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="37768-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="37768-145">Indique si un utilisateur s’est envoyé un élément à lui-même ou à lui-même.</span><span class="sxs-lookup"><span data-stu-id="37768-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="37768-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="37768-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="37768-147">Indique si l'élément a déjà été envoyé.</span><span class="sxs-lookup"><span data-stu-id="37768-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="37768-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="37768-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="37768-149">Indique si l'élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="37768-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="37768-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="37768-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="37768-151">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="37768-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="37768-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="37768-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="37768-153">Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="37768-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="37768-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="37768-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="37768-155">Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.</span><span class="sxs-lookup"><span data-stu-id="37768-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="37768-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="37768-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="37768-157">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37768-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="37768-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="37768-p102">Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  </span><span class="sxs-lookup"><span data-stu-id="37768-p102">Represents the date and time when the event occurs. This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.  </span></span><br/> |
|[<span data-ttu-id="37768-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="37768-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="37768-162">Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="37768-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="37768-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="37768-164">Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.</span><span class="sxs-lookup"><span data-stu-id="37768-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="37768-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="37768-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="37768-p103">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.</span><span class="sxs-lookup"><span data-stu-id="37768-p103">Represents the display string that is used for the contents of the Cc line. This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="37768-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="37768-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="37768-p104">Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.</span><span class="sxs-lookup"><span data-stu-id="37768-p104">Represents the display string that is used for the contents of the To line. This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="37768-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="37768-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="37768-p105">Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  </span><span class="sxs-lookup"><span data-stu-id="37768-p105">Represents a property that is set to **true** if an item has at least one visible attachment. This property is read-only.  </span></span><br/> |
|[<span data-ttu-id="37768-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="37768-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="37768-175">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="37768-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="37768-176">Culture</span><span class="sxs-lookup"><span data-stu-id="37768-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="37768-177">Représente la culture d'un élément donné dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="37768-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="37768-178">UID</span><span class="sxs-lookup"><span data-stu-id="37768-178">UID</span></span>](uid.md) <br/> |<span data-ttu-id="37768-179">Identifie un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-179">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-180">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="37768-180">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="37768-181">Permet d’identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="37768-181">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-182">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="37768-182">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="37768-183">Indique la date et l’heure de création d’une instance d’un objet iCalendar.</span><span class="sxs-lookup"><span data-stu-id="37768-183">Indicates the date and time that an instance of a iCalendar object was created.</span></span>  <br/> |
|[<span data-ttu-id="37768-184">Démarrage</span><span class="sxs-lookup"><span data-stu-id="37768-184">Start</span></span>](start.md) <br/> |<span data-ttu-id="37768-185">Représente le début d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-185">Represents the start of a calendar item.</span></span> <span data-ttu-id="37768-186">Cet élément s’applique uniquement à une seule occurrence d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-186">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-187">Fin</span><span class="sxs-lookup"><span data-stu-id="37768-187">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="37768-188">Représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="37768-188">Represents the end of a duration.</span></span> <span data-ttu-id="37768-189">Cet élément s’applique uniquement à une seule occurrence d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-189">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-190">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="37768-190">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="37768-191">Représente l’heure de début d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-191">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-192">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="37768-192">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="37768-193">Indique si un élément de calendrier ou une demande de réunion représente un événement d’une journée entière.</span><span class="sxs-lookup"><span data-stu-id="37768-193">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="37768-194">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="37768-194">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="37768-195">Représente l’état de disponibilité de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-195">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-196">Emplacement</span><span class="sxs-lookup"><span data-stu-id="37768-196">Location</span></span>](location.md) <br/> |<span data-ttu-id="37768-197">Représente l’emplacement d’une réunion ou d’un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="37768-197">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="37768-198">When</span><span class="sxs-lookup"><span data-stu-id="37768-198">When</span></span>](when.md) <br/> |<span data-ttu-id="37768-199">Fournit des informations sur le moment où un élément de calendrier se produit.</span><span class="sxs-lookup"><span data-stu-id="37768-199">Provides information about when a calendar item occurs.</span></span>  <br/> |
|[<span data-ttu-id="37768-200">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="37768-200">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="37768-201">Indique si l’élément de calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="37768-201">Indicates whether the calendar item is a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="37768-202">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="37768-202">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="37768-203">Indique si un rendez-vous ou une réunion a été annulé.</span><span class="sxs-lookup"><span data-stu-id="37768-203">Indicates whether an appointment or meeting has been canceled.</span></span>  <br/> |
|[<span data-ttu-id="37768-204">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="37768-204">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="37768-205">Indique si un élément de calendrier fait partie d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="37768-205">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="37768-206">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="37768-206">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="37768-207">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="37768-207">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="37768-208">Indique si une demande de réunion a été envoyée aux participants demandés.</span><span class="sxs-lookup"><span data-stu-id="37768-208">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="37768-209">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="37768-209">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="37768-210">Indique si une réponse à un élément est requise.</span><span class="sxs-lookup"><span data-stu-id="37768-210">Indicates whether a response to an item is required.</span></span>  <br/> |
|[<span data-ttu-id="37768-211">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="37768-211">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="37768-212">Représente le type d’occurrence d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-212">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-213">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="37768-213">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="37768-214">Contient l’État ou la réponse à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-214">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-215">Organizer</span><span class="sxs-lookup"><span data-stu-id="37768-215">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="37768-216">Représente l’organisateur d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-216">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="37768-217">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="37768-217">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="37768-218">Représente les participants qui sont requis pour participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-218">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="37768-219">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="37768-219">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="37768-220">Représente les participants qui ne sont pas tenus de participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-220">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="37768-221">Resources</span><span class="sxs-lookup"><span data-stu-id="37768-221">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="37768-222">Représente une ressource planifiée pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-222">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="37768-223">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="37768-223">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="37768-224">Représente le nombre de réunions en conflit avec l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-224">Represents the number of meetings that conflict with the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-225">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="37768-225">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="37768-226">Représente le nombre total d’éléments de calendrier adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-226">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="37768-227">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="37768-227">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="37768-228">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-228">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="37768-229">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="37768-229">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="37768-230">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-230">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="37768-231">Durée (éléments)</span><span class="sxs-lookup"><span data-stu-id="37768-231">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="37768-232">Représente la durée d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-232">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-233">TimeZone (élément)</span><span class="sxs-lookup"><span data-stu-id="37768-233">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="37768-234">Fournit une description textuelle d’un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="37768-234">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="37768-235">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="37768-235">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="37768-236">Représente la date et l’heure auxquelles un participant a répondu à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-236">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="37768-237">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="37768-237">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="37768-238">Spécifie le numéro de séquence d’une version d’un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="37768-238">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="37768-239">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="37768-239">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="37768-240">Spécifie l’état du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="37768-240">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="37768-241">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="37768-241">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="37768-242">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-242">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> <span data-ttu-id="37768-243">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="37768-243">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="37768-244">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="37768-244">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="37768-245">Représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="37768-245">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="37768-246">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="37768-246">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="37768-247">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="37768-247">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="37768-248">Représente la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="37768-248">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="37768-249">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="37768-249">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="37768-250">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="37768-250">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="37768-251">Contient un tableau d’occurrences périodiques d’éléments de calendrier ayant été modifiées afin qu’elles diffèrent de l’élément de masque de récurrence.</span><span class="sxs-lookup"><span data-stu-id="37768-251">Contains an array of recurring calendar item occurrences that have been modified so that they differ from the recurrence master item.</span></span>  <br/> <span data-ttu-id="37768-252">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="37768-252">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="37768-253">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="37768-253">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="37768-254">Contient un tableau d’occurrences supprimées d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="37768-254">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="37768-255">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="37768-255">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="37768-256">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="37768-256">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="37768-257">Représente le fuseau horaire de l’emplacement où la réunion est hébergée.</span><span class="sxs-lookup"><span data-stu-id="37768-257">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="37768-258">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="37768-258">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="37768-259">Représente le fuseau horaire de début de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-259">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-260">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="37768-260">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="37768-261">Représente le fuseau horaire de fin de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-261">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-262">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="37768-262">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="37768-263">Décrit le type de conférence effectuée avec un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-263">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-264">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="37768-264">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="37768-265">Indique si une nouvelle heure de réunion peut être proposée pour une réunion par un participant.</span><span class="sxs-lookup"><span data-stu-id="37768-265">Indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span>  <br/> |
|[<span data-ttu-id="37768-266">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37768-266">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="37768-267">Indique si la réunion est en ligne.</span><span class="sxs-lookup"><span data-stu-id="37768-267">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="37768-268">MeetingWorkspaceUrl,</span><span class="sxs-lookup"><span data-stu-id="37768-268">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="37768-269">Contient l’URL de l’espace de travail de réunion lié par l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-269">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="37768-270">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="37768-270">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="37768-271">Spécifie l’URL d’une réunion Microsoft NetShow online.</span><span class="sxs-lookup"><span data-stu-id="37768-271">Specifies the URL for a Microsoft NetShow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="37768-272">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="37768-272">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="37768-p109">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="37768-p109">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="37768-275">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="37768-275">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="37768-276">Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.</span><span class="sxs-lookup"><span data-stu-id="37768-276">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="37768-277">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="37768-277">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="37768-278">Indique quand un élément a été modifié pour la dernière fois.</span><span class="sxs-lookup"><span data-stu-id="37768-278">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="37768-279">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="37768-279">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="37768-280">Indique si l'élément est associé à un dossier.</span><span class="sxs-lookup"><span data-stu-id="37768-280">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="37768-281">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="37768-281">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="37768-282">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="37768-282">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="37768-283">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="37768-283">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="37768-284">Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour modifier un élément dans Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="37768-284">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="37768-285">ConversationId</span><span class="sxs-lookup"><span data-stu-id="37768-285">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="37768-286">Contient l'identificateur d'un élément ou d'une conversation.</span><span class="sxs-lookup"><span data-stu-id="37768-286">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="37768-287">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="37768-287">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="37768-288">Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.</span><span class="sxs-lookup"><span data-stu-id="37768-288">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37768-289">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37768-289">Parent elements</span></span>

|<span data-ttu-id="37768-290">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37768-290">**Element**</span></span>|<span data-ttu-id="37768-291">**Description**</span><span class="sxs-lookup"><span data-stu-id="37768-291">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37768-292">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="37768-292">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="37768-293">Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-293">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="37768-294">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="37768-294">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="37768-295">Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="37768-295">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="37768-296">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="37768-296">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="37768-297">Identifie tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="37768-297">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="37768-298">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="37768-298">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="37768-299">Identifie un dossier unique à créer dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="37768-299">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="37768-300">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="37768-300">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="37768-301">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-301">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="37768-302">Items</span><span class="sxs-lookup"><span data-stu-id="37768-302">Items</span></span>](items.md) <br/> |<span data-ttu-id="37768-303">Contient un tableau d'éléments.</span><span class="sxs-lookup"><span data-stu-id="37768-303">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="37768-304">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="37768-304">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="37768-305">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="37768-305">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="37768-306">SetItemField</span><span class="sxs-lookup"><span data-stu-id="37768-306">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="37768-307">Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="37768-307">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="37768-308">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="37768-308">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="37768-309">Identifie un élément unique à mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="37768-309">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37768-310">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="37768-310">Text value</span></span>

<span data-ttu-id="37768-311">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37768-311">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37768-312">Remarques</span><span class="sxs-lookup"><span data-stu-id="37768-312">Remarks</span></span>

<span data-ttu-id="37768-313">Lorsqu’un seul élément de calendrier est mis à jour pour devenir un élément de calendrier principal périodique, l’élément [MeetingTimeZone](meetingtimezone.md) doit être spécifié afin de conserver le fuseau horaire d’origine de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="37768-313">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) element must be specified in order to preserve the calendar item's original time zone.</span></span> 
  
<span data-ttu-id="37768-314">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="37768-314">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37768-315">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37768-315">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37768-316">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37768-316">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37768-317">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37768-317">Schema name</span></span>  <br/> |<span data-ttu-id="37768-318">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="37768-318">Types schema</span></span>  <br/> |
|<span data-ttu-id="37768-319">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="37768-319">Validation file</span></span>  <br/> |<span data-ttu-id="37768-320">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37768-320">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37768-321">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37768-321">Can be empty</span></span>  <br/> |<span data-ttu-id="37768-322">False</span><span class="sxs-lookup"><span data-stu-id="37768-322">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37768-323">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37768-323">See also</span></span>



- [<span data-ttu-id="37768-324">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37768-324">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="37768-325">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="37768-325">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

