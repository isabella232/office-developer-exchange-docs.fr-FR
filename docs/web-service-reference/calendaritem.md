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
ms.openlocfilehash: c7b6d4930bc42fbe26d35264e2eae0c986cc8db7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755474"
---
# <a name="calendaritem"></a>CalendarItem

L’élément **CalendarItem** représente un élément de calendrier Exchange. 
  
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

 **CalendarItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contient le flux MIME (Multipurpose Internet Mail Extensions) natif d'un objet représenté au format base64Binary.  <br/> |
|[ID d’élément](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l'identificateur du dossier parent qui contient l'élément ou le dossier.  <br/> |
|[ItemClass](itemclass.md) <br/> |Représente la classe de message d'un élément.  <br/> |
|[Objet](subject.md) <br/> |Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indique le niveau de confidentialité d'un élément.  <br/> |
|[Corps](body.md) <br/> |Représente le contenu réel du corps d'un message.  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Indique la date et l'heure auxquelles un élément de boîte aux lettres a été reçu.  <br/> |
|[Taille](size.md) <br/> |Représente la taille en octets d'un élément. Cette propriété est en lecture seule.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Représente une collection de chaînes qui identifient les catégories auquel appartient un élément dans la boîte aux lettres.  <br/> |
|[Importance](importance.md) <br/> |Décrit l'importance d'un élément.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Représente l'identificateur de l'élément dont cet élément est une réponse.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indique si un élément n’a pas encore été envoyé.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indique si un utilisateur a envoyé un élément pour lui ou elle-même.  <br/> |
|[IsResend](isresend.md) <br/> |Indique si l'élément a déjà été envoyé.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indique si l'élément a été modifié.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
|[Culture](culture.md) <br/> |Représente la culture d'un élément donné dans une boîte aux lettres.  <br/> |
|[UID](uid.md) <br/> |Identifie un élément de calendrier.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Indique la date et l’heure de création d’une instance d’un objet iCalendar.  <br/> |
|[Début](start.md) <br/> |Représente le début d’un élément de calendrier. Cet élément s’applique uniquement à une seule occurrence d’un élément de calendrier.  <br/> |
|[Fin](end-ex15websvcsotherref.md) <br/> |Représente la fin d’une durée. Cet élément s’applique uniquement à une seule occurrence d’un élément de calendrier.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Représente l’heure de début d’origine d’un élément de calendrier.  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |Indique si une demande de réunion ou d’élément de calendrier représente une journée entière.  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |Représente l’état de disponibilité de l’élément de calendrier.  <br/> |
|[Location](location.md) <br/> |Représente l’emplacement d’une réunion ou un rendez-vous.  <br/> |
|[When](when.md) <br/> |Fournit des informations sur un élément de calendrier.  <br/> |
|[IsMeeting](ismeeting.md) <br/> |Indique si l’élément de calendrier est une réunion ou un rendez-vous.  <br/> |
|[IsCancelled](iscancelled.md) <br/> |Indique si un rendez-vous ou une réunion a été annulée.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Indique si un élément de calendrier fait partie d’un élément périodique. Cet élément est en lecture seule.  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |Indique si une demande de réunion a été envoyée aux participants demandés.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Indique si une réponse à un élément est requise.  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |Représente le type d’occurrence d’un élément de calendrier.  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |Contient l’état d’ou réponse à un élément de calendrier.  <br/> |
|[Bibliothèque multimédia](organizer.md) <br/> |Représente l’organisateur d’une réunion.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Représente les participants qui sont nécessaires pour participer à une réunion.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Représente les participants qui ne sont pas indispensables à participer à une réunion.  <br/> |
|[Ressources](resources.md) <br/> |Représente une ressource pour une réunion planifiée.  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |Représente le nombre de réunions entre en conflit avec l’élément de calendrier.  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |Représente le nombre total d’éléments de calendrier sont adjacents à une heure de réunion.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifie tous les éléments qui sont en conflit avec une heure de réunion.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.  <br/> |
|[Durée (éléments)](duration-items.md) <br/> |Représente la durée d’un élément de calendrier.  <br/> |
|[Fuseau horaire (élément)](timezone-item.md) <br/> |Fournit une description d’un fuseau horaire.  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |Représente la date et l’heure lorsqu’un participant a répondu à une demande de réunion.  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |Spécifie le numéro de séquence d’une version d’un rendez-vous.  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |Spécifie l’état du rendez-vous.  <br/> |
|[Périodicité (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité pour les éléments de calendrier et les demandes de réunion.  <br/> Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Contient un tableau d’occurrences d’élément calendrier périodiques qui ont été modifiés afin qu’elles diffèrent de l’élément maître de périodicité.  <br/> Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Contient un tableau d’occurrences supprimés d’un élément de calendrier périodique.  <br/> Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |Représente le fuseau horaire de l’emplacement où se trouve la réunion.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Représente le fuseau horaire de début de l’élément de calendrier.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Représente le fuseau horaire de fin de l’élément de calendrier.  <br/> |
|[ConferenceType](conferencetype.md) <br/> |Décrit le type de conférence est exécutée avec un élément de calendrier.  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |Indique si une nouvelle heure de réunion peut être proposée pour une réunion à un participant.  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |Indique si la réunion en ligne.  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |Contient l’URL de l’espace de travail de réunion qui est liée à l’élément de calendrier.  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Spécifie l’URL d’une réunion en ligne Microsoft NetShow.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.  <br/> |
|[Heure de dernière modification](lastmodifiedtime.md) <br/> |Indique quand un élément a été modifié pour la dernière fois.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indique si l'élément est associé à un dossier.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Représente une URL vers concaténez au point de terminaison Microsoft Office Outlook Web App pour modifier un élément dans Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contient l'identificateur d'un élément ou d'une conversation.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifie tous les éléments qui sont en conflit avec une heure de réunion.  <br/> |
|[Créer (ItemSync)](create-itemsync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d'éléments.  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[Mise à jour (ItemSync)](update-itemsync.md) <br/> |Identifie un élément unique à mettre à jour dans le magasin de client local.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Lorsqu’un élément de calendrier unique est mis à jour pour devenir un élément de calendrier principal périodique, l’élément [MeetingTimeZone](meetingtimezone.md) doit être spécifié afin de conserver le fuseau horaire d’origine de l’élément de calendrier. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
  
[Référence EWS pour Exchange](ews-reference-for-exchange.md)

