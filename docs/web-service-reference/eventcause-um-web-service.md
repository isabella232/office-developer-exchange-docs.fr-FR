---
title: EventCause (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: L’élément EventCause contient une valeur qui indique la cause d’un événement d’appel en réponse à une demande d’opération GetCallInfo (service web de um).
ms.openlocfilehash: 203cefa1a70294bec4d6f4b41aa157da6e639fce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546573"
---
# <a name="eventcause-um-web-service"></a>EventCause (service web de messagerie unifiée)

**L’élément EventCause** contient une valeur qui indique la cause d’un événement d’appel en réponse à une demande [d’opération GetCallInfo (service web de](getcallinfo-operation-um-web-service.md) um). 
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
[EventCause (service web de messagerie unifiée)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md) <br/> |Définit une réponse à une [demande d’opération GetCallInfo (service web de um).](getcallinfo-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- Aucun
    
- UserBusy
    
- NoAnswer
    
- Autres
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)

