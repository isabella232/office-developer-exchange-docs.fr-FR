---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: L’élément ResultType contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou afficher un aperçu uniquement.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829211"
---
# <a name="resulttype"></a>ResultType

L’élément **ResultType** contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou afficher un aperçu uniquement. 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ResultType** est le type de résultat qui est renvoyé pour une recherche de découverte. Valeur texte **StatisticsOnly** renvoie les statistiques de la recherche. Valeur texte **PreviewOnly** retourne des informations d’Aperçu d’élément. 
  
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
   

