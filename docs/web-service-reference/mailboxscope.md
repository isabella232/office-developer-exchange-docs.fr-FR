---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: L’élément MailboxScope identifie si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux.
ms.openlocfilehash: 92823c06d4fe186917c3cfb532eda821bd6a95a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455372"
---
# <a name="mailboxscope"></a>MailboxScope

L’élément **MailboxScope** identifie si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux. 
  
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

La valeur de texte de l’élément **MailboxScope** est la portée de la recherche ou de l’obtention d’éléments dans une conversation sur des boîtes aux lettres principales, des boîtes aux lettres d’archivage ou les boîtes aux lettres principales et d’archivage. Une valeur de texte de **PrimaryOnly** indique une étendue qui cible la boîte aux lettres principale d’un utilisateur. Une valeur de texte de **ArchiveOnly** indique une étendue qui cible la boîte aux lettres d’archivage d’un utilisateur. Une valeur de texte de **All** indique une étendue qui cible à la fois la boîte aux lettres principale et la boîte aux lettres d’archivage. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

