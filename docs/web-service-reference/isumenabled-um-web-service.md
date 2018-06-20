---
title: IsUMEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: L’élément IsUMEnabled indique si une boîte aux lettres est activé pour la messagerie unifiée.
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828113"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (service web de messagerie unifiée)

L’élément **IsUMEnabled** indique si une boîte aux lettres est activé pour la messagerie unifiée. 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus. La valeur **true** indique que la boîte aux lettres est activé pour la messagerie unifiée. La valeur **false** signifie que la boîte aux lettres n’est pas activé pour la messagerie unifiée. 
  
## <a name="remarks"></a>Remarques

Pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée, utilisez l' [opération IsUMEnabled (service web de messagerie unifiée)](isumenabled-operation-um-web-service.md).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération IsUMEnabled (service web de messagerie unifiée)](isumenabled-operation-um-web-service.md)


[Unified Messaging service XML des éléments web pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

