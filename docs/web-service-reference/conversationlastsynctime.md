---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: L’élément ConversationLastSyncTime contient la date et l’heure de dernière synchronisation une conversation. Cet élément doit être présent lorsque vous tentez de supprimer tous les éléments qui ont été reçus jusqu'à l’heure spécifiée dans une conversation.
ms.openlocfilehash: 3b086d69ac0ef307059df4902e65f796c63733d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755645"
---
# <a name="conversationlastsynctime"></a>ConversationLastSyncTime

L’élément **ConversationLastSyncTime** contient la date et l’heure de dernière synchronisation une conversation. Cet élément doit être présent lorsque vous tentez de supprimer tous les éléments qui ont été reçus jusqu'à l’heure spécifiée dans une conversation. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ConversationLastSyncTime](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 **xs : DateTime**
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

La valeur de texte de la **ConversationLastSyncTime** indique la dernière synchronisation de la conversation. 
  
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



[Opération de ApplyConversationAction](applyconversationaction-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

