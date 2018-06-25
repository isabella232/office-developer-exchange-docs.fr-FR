---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: L’élément ActionType Spécifie l’action à effectuer sur le rappel.
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755153"
---
# <a name="actiontype-reminderactiontype"></a>ActionType (ReminderActionType)

L’élément **ActionType** Spécifie l’action à effectuer sur le rappel. 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ActionType** Spécifie l’action à effectuer sur le rappel. La valeur de texte de **faire disparaître** indique le rappel doit être fermé. La valeur de texte de **Répéter** indique que le rappel doit être différé jusqu'à ce que le délai spécifié par l’élément [NewReminderTime](newremindertime.md) . 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ReminderItemAction](reminderitemaction.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

