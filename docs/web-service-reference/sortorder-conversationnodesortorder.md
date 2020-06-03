---
title: OrdreTri (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: L’élément SortOrder spécifie l’ordre de tri utilisé pour le résultat d’une demande GetConversationItems.
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530964"
---
# <a name="sortorder-conversationnodesortorder"></a>OrdreTri (ConversationNodeSortOrder)

L’élément **SortOrder** spécifie l’ordre de tri utilisé pour le résultat d’une demande **GetConversationItems** . 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **SortOrder** est l’ordre dans lequel les conversations sont ordonnées. Une valeur de texte de **TreeOrderAscending** indique que les conversations sont classées en fonction de l’arborescence de conversation dans l’ordre croissant. Une valeur de texte de **TreeOrderDescending** indique que les conversations sont classées en fonction de l’arborescence de conversation dans l’ordre décroissant. Une valeur de texte de **DateOrderAscending** indique que les conversations sont classées en fonction de la date de conversation dans l’ordre croissant. Une valeur de texte de **DateOrderDescending** indique que les conversations sont classées en fonction de la date de conversation dans l’ordre décroissant. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

