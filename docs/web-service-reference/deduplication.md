---
title: Déduplication
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: L’élément déduplication indique si le résultat de recherche doit supprimer les doublons.
ms.openlocfilehash: 3f06bb1dccd0677b7fd43c4ad82eda54a0c3f812
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755833"
---
# <a name="deduplication"></a>Déduplication

L’élément **déduplication** indique si le résultat de recherche doit supprimer les doublons. 
  
```XML
<Deduplication> true | false </Deduplication>
```

**Boolean**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément déduplication indique que les résultats de recherche peuvent contenir pas de doublons. La valeur **false** indique que les résultats de recherche peuvent contenir des éléments en double. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

