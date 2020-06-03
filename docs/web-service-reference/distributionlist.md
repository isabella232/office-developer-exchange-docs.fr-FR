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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457003"
---
# <a name="distributionlist"></a>DistributionList

L’élément **DistributionList** représente une liste de distribution. 
  
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

 **DistributionListType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contient le flux MIME natif d’un objet représenté au format base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contient l’identificateur unique et la clé de modification d’un élément de liste de distribution dans la Banque d’Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent qui contient l’élément de liste de distribution.  <br/> |
|[ItemClass](itemclass.md) <br/> |Représente la classe de message d’un élément de liste de distribution.  <br/> |
|[Objet](subject.md) <br/> |Représente l'objet des éléments de la banque d'informations Exchange et des objets de réponse.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Contient l’état du critère de diffusion d’un élément de liste de distribution.  <br/> |
|[Corps](body.md) <br/> |Représente le contenu réel du corps d’un élément de liste de distribution.  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Contient les éléments ou les fichiers joints à un élément de liste de distribution dans la Banque d’Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Représente la date et l’heure auxquelles un élément de liste de distribution d’une boîte aux lettres a été reçu.  <br/> |
|[Taille](size.md) <br/> |Représente la taille, en octets, d’un élément de liste de distribution. Cette propriété est en lecture seule.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Représente une collection de chaînes qui identifient les catégories auxquelles un élément de liste de distribution appartient à la boîte aux lettres.  <br/> |
|[Importance](importance.md) <br/> |Décrit l’importance d’un élément de liste de distribution.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Représente l’identificateur de l’élément dont cet élément est une réponse.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indique si un élément a été envoyé dans le dossier par défaut de la boîte d'envoi.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indique si un élément n'a pas encore été envoyé.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indique si un utilisateur a envoyé un élément à lui-même.  <br/> |
|[IsResend](isresend.md) <br/> |Indique si l'élément a déjà été envoyé.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indique si l'élément a été modifié.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Représente la collection de tous les en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Indique la date et l'heure auxquelles un élément de boîte aux lettres a été envoyé.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Indique la date et l'heure auxquelles un élément donné de la boîte aux lettres a été créé.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Indique la date et l'heure auxquelles l'événement se produit. Cet élément est utilisé par l'élément [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) afin de déterminer quand le rappel s'affiche.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indique si un rappel a été défini pour un élément dans la banque d'informations Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Représente le nombre de minutes avant un événement lors de l'affichage d'un rappel.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne Cc. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Représente la chaîne d'affichage qui est utilisée pour le contenu de la ligne À. Il s'agit de la chaîne concaténée de tous les noms d'affichage de destinataires À.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Représente une propriété définie sur **true** si un élément comporte au moins une pièce jointe visible. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues d’un élément de liste de distribution.  <br/> |
|[Culture](culture.md) <br/> |Représente la culture d’un élément de liste de distribution dans une boîte aux lettres.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contient le nom d'affichage du dernier utilisateur ayant modifié un élément.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indique quand un élément a été modifié pour la dernière fois.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indique si l'élément est associé à un dossier.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Représente une URL à concaténer au point de terminaison de Microsoft Office Outlook Web App pour lire un élément dans Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Représente une URL à concaténer au point de terminaison d'Outlook Web App pour modifier un élément dans Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contient l'identificateur d'un élément ou d'une conversation.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Représente un fragment HTML ou du texte brut correspondant au corps unique de cette conversation.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom d’affichage d’une liste de distribution.  <br/> |
|[FileAs](fileas.md) <br/> |Représente l’archivage d’une liste de distribution dans le dossier contacts.  <br/> |
|[ContactSource](contactsource.md) <br/> |Indique si le contact se trouve dans la Banque d’information Exchange ou dans les services de domaine Active Directory (AD DS).  <br/> |
|[Membres (MemberListType)](members-memberlisttype.md) <br/> |Contient une liste des membres de la liste de distribution.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Décrit tous les éléments de calendrier qui sont adjacents à une heure de réunion.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à ajouter à une propriété unique d’une liste de distribution pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifie tous les éléments qui sont en conflit avec une heure de réunion.  <br/> |
|[Créer (ItemSync)](create-itemsync.md) <br/> |Identifie une liste de distribution unique à créer dans le magasin client local.  <br/> |
|[Mise à jour (ItemSync)](update-itemsync.md) <br/> |Identifie une liste de distribution unique à mettre à jour dans le magasin client local.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d'éléments.  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d’une propriété unique d’un élément de liste de distribution dans une [opération UpdateItem](updateitem-operation.md).  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

