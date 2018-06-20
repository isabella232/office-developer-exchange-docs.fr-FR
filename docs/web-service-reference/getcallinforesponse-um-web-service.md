---
title: GetCallInfoResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: L’élément GetCallInfoResponse définit une réponse à une demande de (service web de messagerie unifiée) opération GetCallInfo.
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756537"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (service web de messagerie unifiée)

L’élément **GetCallInfoResponse** définit une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|CallState  <br/> |Contient une valeur qui indique l’état d’un appel pour lequel l' [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) les informations demandées.  <br/> |
|EventCause  <br/> |Contient une valeur qui indique la cause d’un événement pour un appel pour lequel l' [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) les informations demandées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[CallState (service web de messagerie unifiée)](callstate-um-web-service.md)
  
[EventCause (service web de messagerie unifiée)](eventcause-um-web-service.md)

