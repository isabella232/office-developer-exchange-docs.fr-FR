---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: L’élément SearchMailboxesResult contient le résultat de la demande SearchMailboxes.
ms.openlocfilehash: dee1e12a6d083ca3f8d3ddb509775b454e3e8fc0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534404"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

**L’élément SearchMailboxesResult** contient le résultat de la **demande SearchMailboxes.** 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 **SearchMailboxesResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Taille (longue)](size-long.md)  |  [PageItemCount](pageitemcount.md)  |  [PageItemSize](pageitemsize.md)  |  [KeywordStats](keywordstats.md)  |  [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)  |  [FailedMailboxes](failedmailboxes.md)  |  [Affinements](refiners.md)  |  [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
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
   

