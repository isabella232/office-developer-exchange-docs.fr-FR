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
# <a name="contact"></a>Contact

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **Contact** représente un contact dans la banque d'informations Exchange. 
  
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

 **ContactItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Nom de l'élément**|**Description**|
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |Représente une collection de chaînes qui identifie les catégories auxquelles un élément de la boîte aux lettres appartient.  <br/> |
|[Importance](importance.md) <br/> |Décrit l'importance d'un élément.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Représente l'identificateur de l'élément dont cet élément est une réponse.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indique si un élément n'a pas encore été envoyé.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indique si un utilisateur s'est envoyé un élément à lui-même.  <br/> |
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
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.  <br/> |
|[Heure de dernière modification](lastmodifiedtime.md) <br/> |Indique quand un élément a été modifié pour la dernière fois.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indique si l'élément est associé à un dossier.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contient l'identificateur d'un élément ou d'une conversation.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.  <br/> |
|[Classer sous](fileas.md) <br/> |Indique comment un contact est classé dans le dossier Contacts.  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |Définit la construction de l'affichage d'un contact.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom d'affichage d'un contact.  <br/> |
|[Prénom](givenname.md) <br/> |Contient le nom d'un contact donné.  <br/> |
|[Initials](initials.md) <br/> |Représente les initiales d'un contact.  <br/> |
|[MiddleName](middlename.md) <br/> |Représente le deuxième prénom d'un contact.  <br/> |
|[Nickname](nickname.md) <br/> |Représente le surnom d'un contact.  <br/> |
|[CompleteName](completename.md) <br/> |Représente le nom complet d'un contact.  <br/> |
|[CompanyName](companyname.md) <br/> |Représente le nom de la société associée à un contact.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Représente une collection d'adresses de messagerie pour un contact.  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contient une collection d'adresses physiques associées à un contact.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Représente une collection de numéros de téléphone pour un contact.  <br/> |
|[AssistantName](assistantname.md) <br/> |Représente un assistant d'un contact.  <br/> |
|[Anniversaire](birthday.md) <br/> |Représente la date de naissance d'un contact.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Représente la page d'accueil (adresse web) d'un contact.  <br/> |
|[Enfants](children.md) <br/> |Contient les noms des enfants d'un contact.  <br/> |
|[Companies](companies.md) <br/> |Représente la collection de sociétés associées à un contact.  <br/> |
|[ContactSource](contactsource.md) <br/> |Indique si le contact se trouve dans la banque d'informations Exchange ou dans le service d'annuaire Active Directory.  <br/> |
|[Department](department.md) <br/> |Représente le service du contact.  <br/> |
|[Génération](generation.md) <br/> |Représente une abréviation de génération suivant le nom complet d'un contact.  <br/> |
|[ImAddresses](imaddresses.md) <br/> |Représente une collection d'adresses de messagerie instantanée pour un contact.  <br/> |
|[JobTitle](jobtitle.md) <br/> |Représente la fonction d'un contact.  <br/> |
|[Manager](manager.md) <br/> |Représente le responsable d'un contact.  <br/> |
|[Mileage](mileage.md) <br/> |Représente le kilométrage d'un contact.  <br/> |
|[OfficeLocation](officelocation.md) <br/> |Représente l'emplacement du bureau d'un contact.  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |Représente les types d'affichage pour les adresses physiques.  <br/> |
|[Profession](profession.md) <br/> |Représente la profession d'un contact.  <br/> |
|[NomEpoux](spousename.md) <br/> |Représente le nom du conjoint d'un contact.  <br/> |
|[Surname](surname.md) <br/> |Représente le nom de famille d'un contact.  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |Contient l'anniversaire de mariage d'un contact.  <br/> |
|[HasPicture](haspicture.md) <br/> |Indique si le contact comporte une photo du contact en pièce jointe.  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |Contient le nom complet d'un contact, y compris son prénom et son nom, orthographié phonétiquement.  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |Contient le prénom d'un contact, orthographié phonétiquement.  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |Contient le nom d'un contact, orthographié phonétiquement.  <br/> |
|[Alias](alias.md) <br/> |Contient l'alias de messagerie d'un contact.  <br/> |
|[Notes (contacts)](notes-contact.md) <br/> |Contient des informations supplémentaires sur le contact.  <br/> |
|[photo](photo.md) <br/> |Contient une valeur qui code la photo d'un contact.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Contient une valeur qui code le certificat SMIME d'un contact.  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |Contient une valeur qui code le certificat Microsoft Exchange d'un contact.  <br/> |
|[DirectoryId](directoryid.md) <br/> |Contient l'identificateur du répertoire d'un contact.  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |Contient des informations SMTP qui identifient la boîte aux lettres du responsable du contact.  <br/> |
|[DirectReports](directreports.md) <br/> |Contient des informations SMTP qui identifient les collaborateurs directs d'un contact.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Nom de l'élément**|**Description**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à ajouter à une propriété unique d'un élément ou d'un dossier lors d'une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifie tous les éléments qui entrent en conflit avec une heure de réunion.  <br/> |
|[Créer (ItemSync)](create-itemsync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d'éléments.  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).  <br/> |
|[Solution](resolution.md) <br/> |Contient une seule entité résolue.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[Mise à jour (ItemSync)](update-itemsync.md) <br/> |Identifie un élément unique à mettre à jour dans le magasin de client local.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

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


[Creating Contacts (Exchange Web Services)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Updating Contacts](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Deleting Contacts](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

