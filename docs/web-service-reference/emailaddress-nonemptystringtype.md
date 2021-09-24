---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: L’élément EmailAddress définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 8740f6f7f67269de86aaa7383a7ad8f3cdf07a4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512995"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

**L’élément EmailAddress** définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres. 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifie la personne à qui l’appelant envoie l’appel.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> | Identifie une adresse de messagerie entièrement résolue.  <br/><br/>Voici quelques expressions XPath à cet élément :<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Les éléments suivants sont des éléments parents supplémentaires de l’élément Mailbox :<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Expéditeur](sender.md) <br/>- [De](from.md) <br/>- [Organisateur](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Résolution](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Attendee](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion par adresse de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

**L’élément EmailAddress** peut représenter des adresses SMTP ou Exchange nom principal (également appelé DN). **L’élément EmailAddress** est le seul élément [Mailbox](mailbox.md) requis. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

