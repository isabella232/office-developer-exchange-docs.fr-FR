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
description: L’élément de boîte aux lettres identifie un objet Active Directory à extension messagerie.
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828258"
---
# <a name="mailbox"></a>Boîte aux lettres

L’élément de **boîte aux lettres** identifie un objet Active Directory à extension messagerie. 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddressType)](name-emailaddresstype.md) <br/> |Définit le nom de l’utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Définit le routage est utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[ID d’élément](itemid.md) <br/> |Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de contacts d’un utilisateur. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Définit une demande pour développer une liste de distribution. <br/> <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Contient un tableau de destinataires d’un élément.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Représente une collection de destinataires qui reçoivent une copie du message.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Représente une collection de destinataires pour recevoir une copie carbone invisible (Cci) d’un message électronique.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifie un tableau d’adresses de messagerie à laquelle les réponses doivent être envoyées.  <br/> |
|[Sender](sender.md) <br/> |Identifie l’expéditeur d’un élément.  <br/> |
|[From](from.md) <br/> |Représente le destinataire à partir de laquelle le message a été envoyé.  <br/> |
|[Bibliothèque multimédia](organizer.md) <br/> |Représente l’organisateur d’une réunion.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Identifie les dossiers de Microsoft Exchange Server 2007 par défaut.  <br/><br/>  Les expressions XPath pour cet élément sont les suivantes : <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Solution](resolution.md) <br/> |Contient une seule entité résolue.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.  <br/> |
|[Attendee](attendee.md) <br/> |Représente les participants et les ressources pour un élément de calendrier.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Définit une demande d’ajout de dossiers gérés pour une boîte aux lettres.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Définit une demande pour ajouter des délégués à une boîte aux lettres.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Définit une demande pour supprimer des délégués d’une boîte aux lettres.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Définit une demande de mise à jour des délégués dans une boîte aux lettres.  <br/> |
|[Reçu par](receivedby.md) <br/> |Décrit les délégués dans un scénario d’accès délégué.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Décrit le principal dans un scénario d’accès délégué.  <br/> |
|[Membre](member-ex15websvcsotherref.md) <br/> |Représente un membre d’une liste de distribution.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les éléments [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) et [ItemId](itemid.md) identifient une boîte aux lettres ou liste de distribution. 

L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifie une boîte aux lettres ou liste de distribution à l’adresse SMTP. 

L’élément [ItemId](itemid.md) identifie une boîte aux lettres par un identificateur d’élément, qui est associé à une boîte aux lettres spécifique. 

L’élément [ItemId](itemid.md) ne peut pas être utilisé pour envoyer un message à une liste de distribution ou un contact dans un dossier public de contacts. Une erreur est levée si elle est utilisée dans une opération CreateItem, UpdateItem ou SendItem lors de la tentative d’envoyer un message à une liste de distribution ou un contact dans un dossier public de contacts. Utilisez l’opération ExpandDL pour obtenir l’adresse SMTP, puis envoyer le message à l’aide de l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) au lieu de l’élément [ItemId](itemid.md) . 
  
Un autre élément, [la boîte aux lettres (disponibilité)](mailbox-availability.md), fournit des informations pour les opérations de disponibilité. 
  
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

