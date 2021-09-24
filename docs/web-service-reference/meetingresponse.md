---
title: MeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingResponse
api_type:
- schema
ms.assetid: 9f798e79-dafd-4d4d-9967-95fd8e5c0502
description: L’élément MeetingResponse représente une réponse de réunion dans le magasin Exchange de réunion.
ms.openlocfilehash: 7fa4c8d618291e69a668fcc2f9ddcd72e9ca28bc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532614"
---
# <a name="meetingresponse"></a>MeetingResponse

**L’élément MeetingResponse** représente une réponse de réunion dans le magasin Exchange de réunion. 
  
```xml
<MeetingResponse>
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
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <ProposedStart/>
   <ProposedEnd/>
</MeetingResponse>
```

 **MeetingResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contient le flux MIME natif d’un objet qui est représenté au format Base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange. Cette propriété est en lecture seule.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l'identificateur du dossier parent qui contient l'élément ou le dossier. Cette propriété est en lecture seule.  <br/> |
|[ItemClass](itemclass.md) <br/> |Représente la classe de message d'un élément.  <br/> |
|[Objet](subject.md) <br/> |Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse. L’objet est limité à 255 caractères.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indique le niveau de confidentialité d'un élément.  <br/> |
|[Body](body.md) <br/> |Représente le contenu réel du corps d'un message.  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Représente les données et l’heure de réception d’un élément dans une boîte aux lettres.  <br/> |
|[Taille](size.md) <br/> |Représente la taille en octets d'un élément. Cette propriété est en lecture seule.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.  <br/> |
|[Importance](importance.md) <br/> |Décrit l'importance d'un élément.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Représente l'identificateur de l'élément dont cet élément est une réponse.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indique si un élément n'a pas encore été envoyé.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indique si un utilisateur lui a envoyé un élément.  <br/> |
|[IsResend](isresend.md) <br/> |Indique si l'élément a déjà été envoyé.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indique si l'élément a été modifié.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Représente la collection de tous les en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Représente la chaîne d’affichage utilisée pour le contenu de la zone Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Représente la chaîne d’affichage utilisée pour le contenu de la zone À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
|[Culture](culture.md) <br/> |Représente la culture d'un élément donné dans une boîte aux lettres.  <br/> |
|[Sender](sender.md) <br/> |Identifie l’expéditeur d’un élément.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Contient un ensemble de destinataires d’un message.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Représente une collection de destinataires qui recevront une copie du message.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Représente une collection de destinataires pour recevoir une copie carbone non voyante ( Bcc) d’un message électronique.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Indique si l’expéditeur d’un élément demande une réception de lecture.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Indique si l’expéditeur d’un élément demande un accusé de réception.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Contient un ID binaire qui représente le fil de discussion auquel appartient ce message.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Représente l’identificateur de conversation.  <br/> |
|[From](from.md) <br/> |Représente l’adresse à partir de laquelle le message a été envoyé.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Représente l’identificateur de message Internet d’un élément.  <br/> |
|[IsRead](isread.md) <br/> |Indique si un message a été lu.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Indique si une réponse à un message électronique est demandée.  <br/> |
|[Références](references.md) <br/> |Représente l’en-tête Usenet utilisé pour mettre en corrélation les réponses avec leurs messages d’origine.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifie un ensemble d’adresses à laquelle les réponses doivent être envoyées.  <br/> |
|[AssociatedCalendarItemId](associatedcalendaritemid.md) <br/> |Représente l’élément de calendrier associé à [un MeetingMessage](meetingmessage.md).  <br/> |
|[IsDelegated](isdelegated.md) <br/> |Indique si une réunion a été gérée par un compte avec un accès délégué.  <br/> |
|[IsOutOfDate](isoutofdate.md) <br/> |Indique si un message de réunion n’est pas à jour.  <br/> |
|[HasBeenProcessed](hasbeenprocessed.md) <br/> |Indique si un élément de message de réunion a été traitée.  <br/> |
|[ResponseType](responsetype.md) <br/> |Représente le type de réponse du destinataire reçu pour une réunion.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Identifie le délégué dans un scénario d’accès délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Identifie le principal dans un scénario d’accès délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ProposedStart](proposedstart.md) <br/> |Spécifie l’heure de début proposée pour une réunion. Cet élément a été introduit dans Microsoft Exchange Server 2013. <br/> |
|[ProposedEnd](proposedend.md) <br/> |Spécifie l’heure de fin proposée pour une réunion. Cet élément a été introduit dans Microsoft Exchange Server 2013. <br/> |
|[UID](uid.md) <br/> |Identifie un élément de calendrier.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Indique la date et l’heure de création d’une instance d’un objet iCalendar.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Identifie tous les éléments de calendrier adjacents à une heure de réunion.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à append à une propriété unique d’un élément lors d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifie tous les éléments qui entrent en conflit avec une heure de réunion.  <br/> |
|[Créer (ItemSync)](create-itemsync.md) <br/> |Identifie un élément unique à créer dans le magasin de clients local.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d'éléments.  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d’éléments à créer.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[Mise à jour (ItemSync)](update-itemsync.md) <br/> |Identifie un élément unique à mettre à jour dans le magasin de client local.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

