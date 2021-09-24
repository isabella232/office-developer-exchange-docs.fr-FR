---
title: GlobalUnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GlobalUnreadCount
api_type:
- schema
ms.assetid: 5e5ccf3e-2f95-4bf9-b915-8b7e59e807a5
description: L’élément GlobalUnreadCount contient le nombre de tous les éléments de conversation non lus dans la boîte aux lettres.
ms.openlocfilehash: 438df5821f1b8c78253b2d328ab4f9e5616295ed
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539815"
---
# <a name="globalunreadcount"></a>GlobalUnreadCount

**L’élément GlobalUnreadCount** contient le nombre de tous les éléments de conversation non lus dans la boîte aux lettres. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversations](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[GlobalUnreadCount](globalunreadcount.md)
  
```XML
<GlobalUnreadCount/>
```

 **xs:int**
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

La valeur de texte de **l’élément GlobalUnreadCount** est une valeur de nombre complet qui représente le nombre de tous les éléments de conversation non lus dans la boîte aux lettres. 
  
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

