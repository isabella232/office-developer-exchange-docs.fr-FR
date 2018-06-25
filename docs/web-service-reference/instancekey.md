---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: L’élément InstanceKey spécifie une clé d’instance d’un élément ou d’une conversation.
ms.openlocfilehash: a0e4f9390d5dc368388b5a20e38796c6c0157a40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827943"
---
# <a name="instancekey"></a>InstanceKey

L’élément **InstanceKey** spécifie une clé d’instance d’un élément ou d’une conversation. 
  
```XML
<InstanceKey></InstanceKey>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
|[Item](item.md) <br/> |Représente un élément générique dans la banque d’informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **InstanceKey** est la clé de l’instance d’un élément ou d’une conversation. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

