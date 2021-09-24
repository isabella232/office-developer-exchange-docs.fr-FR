---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: L’élément ReminderItemAction spécifie l’action d’un élément de rappel.
ms.openlocfilehash: 7cd6898bb44ecd442a02f162008225d904396ba0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512463"
---
# <a name="reminderitemaction"></a>ReminderItemAction

**L’élément ReminderItemAction** spécifie l’action d’un élément de rappel. 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 **ReminderItemActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ActionType (ReminderActionType)](actiontype-reminderactiontype.md)  |  [ItemId](itemid.md)  |  [NewReminderTime](newremindertime.md)
  
### <a name="parent-elements"></a>Éléments parents

[ReminderItemActions](reminderitemactions.md)
  
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



[ReminderItemActions](reminderitemactions.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

