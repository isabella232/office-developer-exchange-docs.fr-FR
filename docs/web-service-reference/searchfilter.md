---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: L’élément SearchFilter contient la chaîne de requête pour filtrer les boîtes aux lettres à renvoyer à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: b71d8dd862e9338afc145545df4cd29e8bcc3dc8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829285"
---
# <a name="searchfilter"></a>SearchFilter

L’élément **SearchFilter** contient la chaîne de requête pour filtrer les boîtes aux lettres à renvoyer à partir d’une demande **GetSearchableMailboxes** . 
  
```XML
<SearchFilter></SearchFilter>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **SearchFilter** est une chaîne de requête aux boîtes aux lettres de filtre pour la recherche de découverte. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

