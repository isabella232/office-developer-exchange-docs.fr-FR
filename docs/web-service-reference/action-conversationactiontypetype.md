---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: L’élément Action contient l’action à effectuer sur la conversation spécifiée par l’élément ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755149"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

L’élément **Action** contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) . 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Action (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une même conversation.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **Action** indique l’action qui sera effectuée sur une conversation. Voici les valeurs possibles de texte et les actions correspondantes : 
  
- **AlwaysCategorize** - les éléments en cours et les nouveaux éléments de la conversation sera automatiquement défini avec les catégories identifiés dans l’élément de [catégories](categories-ex15websvcsotherref.md) . 
    
- **AlwaysDelete** - les éléments en cours et les nouveaux éléments de la conversation seront automatiquement supprimés. Le mode de suppression est défini par l’élément [DeleType](deletetype.md) . 
    
- **AlwaysMove** - les éléments en cours et les nouveaux éléments de la conversation seront automatiquement déplacées vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . 
    
- **Supprimer** : les éléments en cours de la conversation seront supprimés. Les éléments suivants dans la conversation ne seront pas supprimés. Le mode de suppression est défini par l’élément [DeleType](deletetype.md) . 
    
- **Déplacer** - les éléments en cours de la conversation seront déplacées vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . Les éléments suivants dans la conversation ne seront déplacées. 
    
- **Copie** - les éléments en cours de la conversation sont copiées dans le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . Dans la conversation, les éléments suivants ne sont pas copiés. 
    
- **SetReadState** - les éléments de la conversation en cours aura leur état en lecture à définir. L’état de lecture est défini par l’élément [estlu](isread.md) . 
    
- **Indicateur** : les éléments de la conversation en cours aura un indicateur tel que défini par l’élément [indicateur](flag.md) . 
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

