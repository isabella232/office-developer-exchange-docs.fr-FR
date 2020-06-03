---
title: GetCallInfoResponse (service Web de messagerie unifiée)
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
description: L’élément GetCallInfoResponse définit une réponse à une opération GetCallInfo (service Web de messagerie unifiée).
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461204"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (service Web de messagerie unifiée)

L’élément **GetCallInfoResponse** définit une réponse à une [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (service Web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|CallState  <br/> |Contient une valeur qui indique l’état d’un appel pour lequel l' [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) a demandé des informations.  <br/> |
|EventCause  <br/> |Contient une valeur qui indique la cause d’un événement pour un appel pour lequel l' [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) a demandé des informations.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[CallState (service Web de messagerie unifiée)](callstate-um-web-service.md)
  
[EventCause (service Web de messagerie unifiée)](eventcause-um-web-service.md)

