---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'L’élément FindPeople spécifie un ensemble de données utilisées dans une demande FindPeople. Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), un affichage d’élément de page indexé, une restriction (facultative), une restriction d’agrégation (facultative), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultative).'
ms.openlocfilehash: 44070c79ad5d1615929a6169d1808cf365b7cab4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535162"
---
# <a name="findpeople"></a>FindPeople

**L’élément FindPeople** spécifie un ensemble de données utilisées dans une demande FindPeople. Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), un affichage d’élément de page indexé, une restriction (facultative), une restriction d’agrégation (facultative), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultative). 
  
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

[PersonaShape](personashape.md)  |  [IndexedPageItemView](indexedpageitemview.md)  |  [Restriction](restriction.md)  |  [AggregationRestriction](aggregationrestriction.md)  |  [SortOrder](sortorder.md)  |  [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [QueryString (QueryStringType)](querystring-querystringtype.md)
  
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
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

