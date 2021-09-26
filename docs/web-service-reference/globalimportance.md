---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: L’élément GlobalImportance contient l’importance agrégée pour tous les éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: 52564ee9d3431ffcacf15fd1731d5d50f5323db7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547385"
---
# <a name="globalimportance"></a>GlobalImportance

**L’élément GlobalImportance** contient l’importance agrégée pour tous les éléments de conversation dans une boîte aux lettres. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversations](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[GlobalImportance](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 **ImportanceChoicesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles pour cet élément sont les suivantes :
  
- Faible
    
- Normal
    
- Élevé
    
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



[FindConversation Operation](findconversation-operation.md)
  
[Opération de ApplyConversationAction](applyconversationaction-operation.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

