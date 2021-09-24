---
title: CallId (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: L’élément CallId contient la valeur qui représente l’identificateur de l’appel dans une demande GetCallInfo (service web de la um) ou disconnect (service web de um).
ms.openlocfilehash: c19f1061d81bf7683fd2c84fb1c6968826046be6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522031"
---
# <a name="callid-um-web-service"></a>CallId (service web de messagerie unifiée)

**L’élément CallId** contient la valeur qui représente l’identificateur de l’appel dans une demande [GetCallInfo (service web de](getcallinfo-um-web-service.md) la um) ou disconnect [(service web de](disconnect-um-web-service.md) um). 
  
[GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md)
  
[CallId (service web de messagerie unifiée)](callid-um-web-service.md)
  
[Disconnect (service web de messagerie unifiée)](disconnect-um-web-service.md)
  
[CallId (service web de messagerie unifiée)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md) <br/> |Définit une demande pour obtenir des informations sur un appel.  <br/> |
|[Disconnect (service web de messagerie unifiée)](disconnect-um-web-service.md) <br/> |Définit une demande de déconnexion d’un appel.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte représente l’identificateur d’un appel.
  
## <a name="remarks"></a>Remarques

Pour initialiser un appel, utilisez l’opération [PlayOnPhone (service web](playonphone-operation-um-web-service.md) de um) ou [l’opération PlayOnPhoneGreeting (service web de la um).](playonphonegreeting-operation-um-web-service.md) Utilisez la valeur de texte renvoyée dans les éléments [PlayOnPhoneResponse (service web](playonphoneresponse-um-web-service.md) de messagerie unie) ou [PlayOnPhoneGreetingResponse (service web](playonphonegreetingresponse-um-web-service.md) de messagerie unie) pour la valeur de texte de l’élément **CallId.** 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[Opération de déconnexion (service web de messagerie unifiée)](disconnect-operation-um-web-service.md)
  
[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

