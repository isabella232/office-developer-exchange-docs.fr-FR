---
title: CallId (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: L’élément CallId contient la valeur qui représente l’identificateur de l’appel dans une demande de GetCallInfo (service Web de messagerie unifiée) ou de déconnexion (service Web de messagerie unifiée).
ms.openlocfilehash: 5d5f596d4a98cbfb4b53be04278dae2305fc10c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529454"
---
# <a name="callid-um-web-service"></a>CallId (service Web de messagerie unifiée)

L’élément **CallId** contient la valeur qui représente l’identificateur de l’appel dans une demande de [GetCallInfo (service Web de messagerie unifiée)](getcallinfo-um-web-service.md) ou de [déconnexion (service Web de messagerie unifiée)](disconnect-um-web-service.md) . 
  
[GetCallInfo (service Web de messagerie unifiée)](getcallinfo-um-web-service.md)
  
[CallId (service Web de messagerie unifiée)](callid-um-web-service.md)
  
[Disconnect (service Web de messagerie unifiée)](disconnect-um-web-service.md)
  
[CallId (service Web de messagerie unifiée)](callid-um-web-service.md)
  
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
|[GetCallInfo (service Web de messagerie unifiée)](getcallinfo-um-web-service.md) <br/> |Définit une demande pour obtenir des informations sur un appel.  <br/> |
|[Disconnect (service Web de messagerie unifiée)](disconnect-um-web-service.md) <br/> |Définit une demande de déconnexion d’un appel.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte représente l’identificateur d’un appel.
  
## <a name="remarks"></a>Remarques

Pour initialiser un appel, utilisez l' [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) ou [PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md). Utilisez la valeur de texte qui est renvoyée dans les éléments [PlayOnPhoneResponse (service Web de messagerie unifiée)](playonphoneresponse-um-web-service.md) ou [PlayOnPhoneGreetingResponse (service Web de messagerie unifiée)](playonphonegreetingresponse-um-web-service.md) pour la valeur de texte de l’élément **CallId** . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[Opération de déconnexion (service Web de messagerie unifiée)](disconnect-operation-um-web-service.md)
  
[Opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

