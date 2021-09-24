---
title: GetCallInfoResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: L’élément GetCallInfoResponse définit une réponse à une demande d’opération GetCallInfo (service web de um).
ms.openlocfilehash: 4b631bdee87e57c1612e906c725adabb9f9ce63e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526188"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (service web de messagerie unifiée)

**L’élément GetCallInfoResponse** définit une réponse à une [demande d’opération GetCallInfo (service web de um).](getcallinfo-operation-um-web-service.md) 
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
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
|CallState  <br/> |Contient une valeur qui indique l’état d’un appel pour lequel l’opération [GetCallInfo (service web de](getcallinfo-operation-um-web-service.md) la um) a demandé des informations.  <br/> |
|EventCause  <br/> |Contient une valeur qui indique la cause d’un événement pour un appel pour lequel l’opération [GetCallInfo (service web de](getcallinfo-operation-um-web-service.md) la um) a demandé des informations.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[CallState (service web de messagerie unifiée)](callstate-um-web-service.md)
  
[EventCause (service web de messagerie unifiée)](eventcause-um-web-service.md)

