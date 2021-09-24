---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: L’élément Action contient l’action à effectuer sur la conversation spécifiée par l’élément ConversationId.
ms.openlocfilehash: e75d9d5df75894d1de9831b0022269e7ace4fa63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514892"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

**L’élément Action** contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId.](conversationid.md) 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Action (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une seule conversation.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément Action** indique l’action à effectuer sur une conversation. Les valeurs de texte possibles et les actions correspondantes sont les suivantes : 
  
- **AlwaysCategorize** : les éléments actuels et les nouveaux éléments de la conversation seront automatiquement défini avec les catégories identifiées dans [l’élément Categories.](categories-ex15websvcsotherref.md) 
    
- **AlwaysDelete** : les éléments actuels et les nouveaux éléments de la conversation sont automatiquement supprimés. Le mode de suppression est définie par [l’élément DeleteType.](deletetype.md) 
    
- **AlwaysMove** : les éléments actuels et les nouveaux éléments de la conversation sont automatiquement déplacés vers le dossier identifié par l’élément [DestinationFolderId.](destinationfolderid.md) 
    
- **Supprimer** : les éléments actuels de la conversation seront supprimés. Les éléments suivants de la conversation ne seront pas supprimés. Le mode de suppression est définie par [l’élément DeleteType.](deletetype.md) 
    
- **Move** : les éléments actuels de la conversation sont déplacés vers le dossier identifié par l’élément [DestinationFolderId.](destinationfolderid.md) Les éléments suivants de la conversation ne seront pas déplacés. 
    
- **Copier** : les éléments actuels de la conversation seront copiés dans le dossier identifié par l’élément [DestinationFolderId.](destinationfolderid.md) Les éléments suivants de la conversation ne seront pas copiés. 
    
- **SetReadState** : l’état de lecture des éléments actuels de la conversation est réglé. L’état de lecture est définie par [l’élément IsRead.](isread.md) 
    
- **Indicateur** : les éléments actuels de la conversation auront un indicateur défini par [l’élément Flag.](flag.md) 
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

