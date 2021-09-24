---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: L’élément MailboxScope indique si une recherche ou une extraction d’une conversation doit s’étendre à la boîte aux lettres principale, à la boîte aux lettres d’archivage ou à la boîte aux lettres principale et d’archivage.
ms.openlocfilehash: 705c72ae2aefbb16599f392eb712d080668490b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522879"
---
# <a name="mailboxscope"></a>MailboxScope

**L’élément MailboxScope** indique si une recherche ou une extraction d’une conversation doit s’étendre à la boîte aux lettres principale, à la boîte aux lettres d’archivage ou à la boîte aux lettres principale et d’archivage. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[FindConversation](findconversation.md)  |  [GetConversationItems](getconversationitems.md)  |  [Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **MailboxScope** est l’étendue de recherche ou d’obtention d’éléments dans une conversation entre les boîtes aux lettres principales, les boîtes aux lettres d’archivage ou les boîtes aux lettres principales et d’archivage. Une valeur de texte **PrimaryOnly indique** une étendue qui cible la boîte aux lettres principale d’un utilisateur. La valeur texte **ArchiveOnly** indique une étendue qui cible la boîte aux lettres d’archivage d’un utilisateur. La valeur texte **All** indique une étendue qui cible à la fois la boîte aux lettres principale et la boîte aux lettres d’archivage. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

