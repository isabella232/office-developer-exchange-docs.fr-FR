---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: L’élément ResultType contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou aperçu uniquement.
ms.openlocfilehash: 6617c8b4b64cd9b6728317d7247bcc5378e488f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465281"
---
# <a name="resulttype"></a>ResultType

L’élément **ResultType** contient le type de recherche à effectuer. Le type de recherche peut être statistiques uniquement ou aperçu uniquement. 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxesResult](searchmailboxesresult.md)  |  [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **ResultType** est le type de résultat renvoyé pour une recherche de découverte. Une valeur de texte de **StatisticsOnly** renverra les statistiques de la recherche. Une valeur de texte de **PreviewOnly** renverra des informations d’aperçu d’élément. 
  
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
   

