---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'L’élément FindPeople spécifie un ensemble de données utilisé dans une demande FindPeople. Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), une vue d’élément de page indexée, une restriction (facultative), une restriction d’agrégation (facultatif), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultatif).'
ms.openlocfilehash: 4777601b7146ec857b5c79fa9d4ced59a7247889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462900"
---
# <a name="findpeople"></a>FindPeople

L’élément **FindPeople** spécifie un ensemble de données utilisé dans une demande FindPeople. Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), une vue d’élément de page indexée, une restriction (facultative), une restriction d’agrégation (facultatif), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultatif). 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 **FindPeopleType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[PersonaShape](personashape.md)  |  [IndexedPageItemView](indexedpageitemview.md)  |  [Restriction](restriction.md)  |  [AggregationRestriction](aggregationrestriction.md)  |  [OrdreTri (SortOrder](sortorder.md)  |  ) [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [QueryString (QueryStringType)](querystring-querystringtype.md)
  
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
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

