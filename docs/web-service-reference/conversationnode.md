---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: L’élément ConversationNode spécifie un nœud dans une conversation.
ms.openlocfilehash: 074209c1b5669db8dd1ea4ba7f9dea064628afbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462702"
---
# <a name="conversationnode"></a>ConversationNode

L’élément **ConversationNode** spécifie un nœud dans une conversation. 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 **ConversationNodeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[InternetMessageId](internetmessageid.md) <br/> |Représente l’identificateur de message Internet d’un élément.  <br/> |
|[ParentInternetMessageId](parentinternetmessageid.md) <br/> |Spécifie l’identificateur du message Internet parent.  <br/> |
|[ItemIds (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Spécifie tous les éléments du nœud conversation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationNodes](conversationnodes.md) <br/> |Spécifie une collection de nœuds de conversation.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

