---
title: MissedCallNotificationEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- MissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 8e6bf0b1-ff76-474c-ac0f-621b6ab89212
description: L’élément MissedCallNotificationEnabled contient une valeur qui indique si une notification d’appel manqué est activée dans une réponse à une demande d’opération (service web de messagerie unifiée) GetUMProperties.
ms.openlocfilehash: 6bebbe6eeb40a259f0c51355a3fea838e8671706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828477"
---
# <a name="missedcallnotificationenabled-um-web-service"></a>MissedCallNotificationEnabled (service web de messagerie unifiée)

L’élément **MissedCallNotificationEnabled** contient une valeur qui indique si une notification d’appel manqué est activée dans une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)
  
[MissedCallNotificationEnabled (service web de messagerie unifiée)](missedcallnotificationenabled-um-web-service.md)
  
```xml
<MissedCallNotificationEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md) <br/> |Définit une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de type Boolean texte est requise. Les valeurs possibles sont les suivantes :
  
- True
    
- Faux
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md)
  
[Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)](setmissedcallnotificationenabled-operation-um-web-service.md)

