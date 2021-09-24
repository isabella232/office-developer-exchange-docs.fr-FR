---
title: Conversation (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: L’élément Conversation représente une conversation unique renvoyée dans une réponse GetConversationItems.
ms.openlocfilehash: 9c7faf9c06c1476bca688e831f452e711a89f10f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533892"
---
# <a name="conversation-conversationrequesttype"></a>Conversation (ConversationRequestType)

**L’élément Conversation** représente une conversation unique renvoyée dans une **réponse GetConversationItems.** 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ConversationId](conversationid.md)  |  [SyncState (base64Binary)](syncstate-base64binary.md)
  
### <a name="parent-elements"></a>Éléments parents

[Conversations](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

