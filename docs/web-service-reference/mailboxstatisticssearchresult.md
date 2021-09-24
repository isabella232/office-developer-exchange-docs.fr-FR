---
title: MailboxStatisticsSearchResult
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 73499df7-3d50-4e39-895d-6e15dd8b2777
description: L’élément MailboxStatisticsSearchResult contient les résultats d’une recherche par mot clé.
ms.openlocfilehash: f73a789d0931e9c15d052444f6a191ae70cbff24
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511109"
---
# <a name="mailboxstatisticssearchresult"></a>MailboxStatisticsSearchResult

**L’élément MailboxStatisticsSearchResult** contient les résultats d’une recherche par mot clé. 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

**MailboxStatisticsSearchResultType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[UserMailbox](usermailbox.md)  |  [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindMailboxStatisticsByKeywordsResponseMessage](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

