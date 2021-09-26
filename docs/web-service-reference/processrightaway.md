---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: L’élément ProcessRightAway indique si la réponse est envoyée dès que l’action commence le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée. Cet élément doit être présent pour que la réponse soit envoyée asynchrone à l’action demandée.
ms.openlocfilehash: 5546bbff4e1e1ef17eee94f1f42492fbf070fe59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542994"
---
# <a name="processrightaway"></a>ProcessRightAway

**L’élément ProcessRightAway** indique si la réponse est envoyée dès que l’action commence le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée. Cet élément doit être présent pour que la réponse soit envoyée asynchrone à l’action demandée. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ProcessRightAway](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs:boolean**
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

Une valeur de texte **true** indique que la réponse est envoyée dès que l’action commence le traitement sur le serveur. Une valeur de texte **false** indique que la réponse est envoyée une fois l’action terminée. 
  
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



[Opération de ApplyConversationAction](applyconversationaction-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

