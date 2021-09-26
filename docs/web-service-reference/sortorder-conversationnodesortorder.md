---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: L’élément SortOrder spécifie l’ordre de tri utilisé pour le résultat d’une demande GetConversationItems.
ms.openlocfilehash: 0091968f1359b0cf744525139b5c6a8cf1687d81
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544674"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

**L’élément SortOrder** spécifie l’ordre de tri utilisé pour le résultat d’une **demande GetConversationItems.** 
  
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

La valeur de texte de **l’élément SortOrder** est l’ordre dans lequel les conversations sont triées. Une valeur de texte **TreeOrderAscending** indique que les conversations sont triées selon l’arborescence de conversation dans l’ordre croissant. Une valeur de texte **TreeOrderDescending** indique que les conversations sont ordonnées en fonction de l’arborescence de conversation dans l’ordre décroit. Une valeur de texte **DateOrderAscending** indique que les conversations sont triées par ordre croissant en fonction de la date de la conversation. Une valeur de texte **DateOrderDescending** indique que les conversations sont ordonnées en fonction de la date de conversation dans l’ordre décroit. 
  
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
   

