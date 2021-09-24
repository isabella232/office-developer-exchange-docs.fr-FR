---
title: SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5d8c367a-67e9-43b3-8be0-6362d2152431
description: L’élément SearchMailboxes indique le début de la demande SearchMailboxes.
ms.openlocfilehash: 3c734e49869a17fa58252668ddae606d702f3047
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521592"
---
# <a name="searchmailboxes"></a>SearchMailboxes

**L’élément SearchMailboxes** indique le début de la **demande SearchMailboxes.** 
  
```XML
<SearchMailboxes>
   <SearchQueries/>
   <ResultType/>
   <PreviewItemResponseShape/>
   <SortBy/>
   <Language/>
   <Deduplication/>
   <PageSize/>
   <PageItemReference/>
   <PageDirection/>
</SearchMailboxes>
```

 **SearchMailboxesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [PreviewItemResponseShape](previewitemresponseshape.md)  |  [SortBy](sortby.md)  |  [Langue](language.md)  |  [Déduplication](deduplication.md)  |  [PageSize](pagesize.md)  |  [PageItemReference](pageitemreference.md)  |  [PageDirection](pagedirection.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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
   

