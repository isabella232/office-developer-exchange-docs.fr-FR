---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: L’élément SearchScope spécifie l’étendue d’une recherche.
ms.openlocfilehash: df11c8db418ac90d1166030aeed3672c0b810052
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466863"
---
# <a name="searchscope"></a>SearchScope

L’élément **SearchScope** spécifie l’étendue d’une recherche. 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **MailboxSearchLocationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MailboxSearchScope](mailboxsearchscope.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **SearchScope** indique le type de boîte aux lettres qui fait l’objet d’une recherche de découverte. Une valeur de texte de **PrimaryOnly** indique que la boîte aux lettres principale fait l’objet d’une recherche. Une valeur de texte de **ArchiveOnly** indique que la boîte aux lettres d’archivage est recherchée. Une valeur de texte de **All** indique que la recherche s’effectue dans les boîtes aux lettres principale et d’archivage. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

