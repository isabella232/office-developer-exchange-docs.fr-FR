---
title: CallState (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: L’élément CallState contient une valeur qui indique l’état d’un appel.
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755489"
---
# <a name="callstate-um-web-service"></a>CallState (service web de messagerie unifiée)

L’élément **CallState** contient une valeur qui indique l’état d’un appel. 
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
[CallState (service web de messagerie unifiée)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md) <br/> |Définit une réponse à une [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md).  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs possibles sont les suivantes :
  
- Inactif
    
- Connexion
    
- Alerté
    
- Connecté
    
- Déconnecté
    
- Entrant
    
- Transfert
    
- Transfert
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)

