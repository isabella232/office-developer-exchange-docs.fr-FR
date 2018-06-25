---
title: EventCause (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: L’élément EventCause contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une demande de (service web de messagerie unifiée) opération GetCallInfo.
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756219"
---
# <a name="eventcause-um-web-service"></a>EventCause (service web de messagerie unifiée)

L’élément **EventCause** contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
[EventCause (service web de messagerie unifiée)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md) <br/> |Définit une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs possibles sont les suivantes :
  
- Aucun
    
- UserBusy
    
- NoAnswer
    
- Other
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)

