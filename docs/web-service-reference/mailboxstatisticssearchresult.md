---
title: MailboxStatisticsSearchResult
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 73499df7-3d50-4e39-895d-6e15dd8b2777
description: L’élément MailboxStatisticsSearchResult contient les résultats d’une recherche par mot-clé.
ms.openlocfilehash: 5b40622cf15596d7ab8a7fa09c9a1998092c3ee7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828302"
---
# <a name="mailboxstatisticssearchresult"></a>MailboxStatisticsSearchResult

L’élément **MailboxStatisticsSearchResult** contient les résultats d’une recherche par mot-clé. 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

**MailboxStatisticsSearchResultType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[UserMailbox](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindMailboxStatisticsByKeywordsResponseMessage](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

