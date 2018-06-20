---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: L’élément SortOrder Spécifie l’ordre de tri pour le résultat d’une demande GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829520"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

L’élément **SortOrder** Spécifie l’ordre de tri pour le résultat d’une demande **GetConversationItems** . 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **SortOrder** est l’ordre dans lequel les conversations commandée. Une valeur texte **TreeOrderAscending** indique que les conversations sont triées en fonction de l’arborescence de la conversation dans l’ordre croissant. Une valeur texte **TreeOrderDescending** indique que les conversations sont triées en fonction de l’arborescence de la conversation dans l’ordre décroissant. Une valeur texte **DateOrderAscending** indique que les conversations sont triées en fonction de la date de la conversation dans l’ordre croissant. Une valeur texte **DateOrderDescending** indique que les conversations sont triées en fonction de la date de la conversation dans l’ordre décroissant. 
  
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
   

