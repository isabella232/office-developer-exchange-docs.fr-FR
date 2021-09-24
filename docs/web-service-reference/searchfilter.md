---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: L’élément SearchFilter contient la chaîne de requête pour filtrer les boîtes aux lettres à retourner à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: 19bb3109942c9a3064cbeaae4a19380d97c94feb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509356"
---
# <a name="searchfilter"></a>SearchFilter

**L’élément SearchFilter** contient la chaîne de requête pour filtrer les boîtes aux lettres à retourner à partir d’une **demande GetSearchableMailboxes.** 
  
```XML
<SearchFilter></SearchFilter>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément SearchFilter** est une chaîne de requête pour filtrer les boîtes aux lettres pour la recherche de découverte. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

