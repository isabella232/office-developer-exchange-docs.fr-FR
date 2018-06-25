---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: L’élément EmailAddress définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756107"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

L’élément **EmailAddress** définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres. 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifie les personnes envoie par l’appelant.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> | Identifie une adresse de messagerie entièrement résolu.  <br/><br/>Certaines expressions XPath pour cet élément sont les suivantes :<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Éléments supplémentaires parent de l’élément de boîte aux lettres sont les suivantes :<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Expéditeur](sender.md) <br/>- [De](from.md) <br/>- [Bibliothèque multimédia](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Résolution](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Participant](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion à l’adresse de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

L’élément **EmailAddress** peut représenter SMTP ou unique Exchange hérité adresses nom (DN). L’élément **EmailAddress** est le seul élément de [boîte aux lettres](mailbox.md) requis. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

