---
title: Boîte aux lettres
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: L’élément Mailbox identifie un objet Active Directory à messagerie.
ms.openlocfilehash: 8065c0472c3b847d538422aa77cd93f75d919a9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535002"
---
# <a name="mailbox"></a>Boîte aux lettres

**L’élément Mailbox** identifie un objet Active Directory à messagerie. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Définit le nom de l’utilisateur de la boîte aux lettres. Cet élément est facultatif.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Définit le routage utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[ItemId](itemid.md) <br/> |Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires du dossier contacts d’un utilisateur. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Définit une demande de développement d’une liste de distribution. <br/> <br/> Voici l’expression XPath de cet élément : ` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Contient un tableau de destinataires d’un élément.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Représente une collection de destinataires qui recevront une copie du message.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Représente une collection de destinataires pour recevoir une copie carbone non voyante ( Bcc) d’un message électronique.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifie un tableau d’adresses de messagerie à laquelle les réponses doivent être envoyées.  <br/> |
|[Sender](sender.md) <br/> |Identifie l’expéditeur d’un élément.  <br/> |
|[From](from.md) <br/> |Représente l’adresse à partir de laquelle le message a été envoyé.  <br/> |
|[Organizer](organizer.md) <br/> |Représente l’organisateur d’une réunion.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Identifie les dossiers Microsoft Exchange Server 2007 par défaut.  <br/><br/>  Les expressions XPath de cet élément sont les suivantes : <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Solution](resolution.md) <br/> |Contient une seule entité résolue.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contient un tableau de boîtes aux lettres contenues dans une liste de distribution.  <br/> |
|[Attendee](attendee.md) <br/> |Représente les participants et les ressources pour un élément de calendrier.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Définit une demande d’ajout de dossiers gérés à une boîte aux lettres.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Définit une demande d’ajout de délégués à une boîte aux lettres.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Définit une demande de suppression de délégués d’une boîte aux lettres.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Définit une demande de mise à jour des délégués dans une boîte aux lettres.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Décrit le délégué dans un scénario d’accès délégué.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Décrit le principal dans un scénario d’accès délégué.  <br/> |
|[Membre](member-ex15websvcsotherref.md) <br/> |Représente un membre d’une liste de distribution.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les [éléments EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) et [ItemId](itemid.md) identifient une boîte aux lettres ou une liste de distribution. 

[L’élément EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifie une boîte aux lettres ou une liste de distribution par adresse SMTP. 

[L’élément ItemId](itemid.md) identifie une boîte aux lettres par un identificateur d’élément, qui est associé à une boîte aux lettres particulière. 

[L’élément ItemId](itemid.md) ne peut pas être utilisé pour envoyer un message à une liste de distribution ou à un contact dans un dossier de contacts publics. Une erreur est lancée si elle est utilisée dans une opération CreateItem, UpdateItem ou SendItem lorsqu’une tentative d’envoi d’un message à une liste de distribution ou à un contact dans un dossier public de contacts est tentée. Utilisez l’opération ExpandDL pour obtenir l’adresse SMTP, puis envoyez le message à l’aide de l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) au lieu de l’élément [ItemId.](itemid.md) 
  
Un autre élément, [Mailbox (Availability)](mailbox-availability.md), fournit des informations pour les opérations de disponibilité. 
  
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

