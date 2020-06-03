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
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463131"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

L’élément **EmailAddress** définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres. 
  
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
|[Actionas](actingas.md) <br/> |Identifie les personnes qui envoient l’appelant.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> | Identifie une adresse de messagerie entièrement résolue.  <br/><br/>Voici quelques expressions XPath sur cet élément :<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Les éléments suivants sont des éléments parents supplémentaires de l’élément Mailbox :<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Expéditeur](sender.md) <br/>- [De](from.md) <br/>- [Organiser](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Résolution](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Participant](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion par adresse de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

L’élément **EmailAddress** peut représenter des adresses SMTP ou des noms uniques Exchange hérités (également appelés DN). L’élément **EmailAddress** est le seul élément de [boîte aux lettres](mailbox.md) obligatoire. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

