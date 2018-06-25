---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: L’élément MailboxScope indique si une recherche ou extraction d’une conversation doit s’étendent à la boîte aux lettres principale, boîte aux lettres d’archivage ou à la fois le serveur principal et d’archivage de boîte aux lettres.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828293"
---
# <a name="mailboxscope"></a>MailboxScope

L’élément **MailboxScope** indique si une recherche ou extraction d’une conversation doit s’étendent à la boîte aux lettres principale, boîte aux lettres d’archivage ou à la fois le serveur principal et d’archivage de boîte aux lettres. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **MailboxScope** est l’étendue de recherche ou de l’obtention d’éléments dans une conversation entre deux boîtes aux lettres principales, archiver des boîtes aux lettres ou les deux principal et archiver des boîtes aux lettres. La valeur texte **PrimaryOnly** indique une étendue qui cible la boîte aux lettres principale pour un utilisateur. La valeur texte **ArchiveOnly** indique une étendue qui cible la boîte aux lettres d’archivage pour un utilisateur. Une valeur de texte de **toutes les** indique une étendue qui cible la boîte aux lettres principale et la boîte aux lettres d’archive. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

