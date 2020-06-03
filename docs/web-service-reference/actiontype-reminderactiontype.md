---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: L’élément ActionType spécifie l’action à effectuer sur le rappel.
ms.openlocfilehash: 5c62b2dd945b23a5ff2bb824385c45dbc617a5a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465057"
---
# <a name="actiontype-reminderactiontype"></a>ActionType (ReminderActionType)

L’élément **ActionType** spécifie l’action à effectuer sur le rappel. 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **ActionType** spécifie l’action à effectuer sur le rappel. La valeur **texte de la** propriété Reverse indique que le rappel doit être fermé. La valeur de la propriété **SNOOZE** indique que le rappel doit être retardé jusqu’à l’heure spécifiée par l’élément [NewReminderTime](newremindertime.md) . 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ReminderItemAction](reminderitemaction.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

