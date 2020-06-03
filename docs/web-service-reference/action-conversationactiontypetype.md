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
description: L’élément action contient l’action à effectuer sur la conversation spécifiée par l’élément ConversationId.
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527543"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

L’élément **action** contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) . 
  
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
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une conversation unique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **action** indique l’action à effectuer sur une conversation. Voici les valeurs de texte possibles et les actions correspondantes : 
  
- **AlwaysCategorize** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement définis avec les catégories identifiées dans l’élément [categories](categories-ex15websvcsotherref.md) . 
    
- **AlwaysDelete** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement supprimés. Le mode de suppression est défini par l’élément [DeleteType](deletetype.md) . 
    
- **AlwaysMove** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement déplacés vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . 
    
- **Supprimer** : les éléments actuels de la conversation seront supprimés. Les éléments suivants de la conversation ne seront pas supprimés. Le mode de suppression est défini par l’élément [DeleteType](deletetype.md) . 
    
- **Move** : les éléments actuels de la conversation seront déplacés vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . Les éléments suivants de la conversation ne seront pas déplacés. 
    
- **Copier** : les éléments actuels de la conversation seront copiés dans le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) . Les éléments suivants de la conversation ne seront pas copiés. 
    
- **SetReadState** : l’état de lecture est défini pour les éléments actuels de la conversation. L’état de lecture est défini par l’élément [IsRead](isread.md) . 
    
- **Flag** : les éléments actuels de la conversation auront un indicateur défini par l’élément [Flag](flag.md) . 
    
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

