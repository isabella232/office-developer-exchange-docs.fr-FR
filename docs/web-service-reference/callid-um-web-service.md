---
title: ID d’appel (service web de messagerie unifiée)
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
description: L’élément CallId contient la valeur qui représente l’identificateur de l’appel dans une demande de (service web de messagerie unifiée) GetCallInfo ou d’une requête (service web de messagerie unifiée) de déconnexion.
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755488"
---
# <a name="callid-um-web-service"></a>ID d’appel (service web de messagerie unifiée)

L’élément **CallId** contient la valeur qui représente l’identificateur de l’appel dans une demande de [GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md) ou une demande de [déconnexion (service web de messagerie unifiée)](disconnect-um-web-service.md) . 
  
[GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md)
  
[ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)
  
[Déconnecter (service web de messagerie unifiée)](disconnect-um-web-service.md)
  
[ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md) <br/> |Définit une demande pour obtenir des informations relatives à un appel.  <br/> |
|[Déconnecter (service web de messagerie unifiée)](disconnect-um-web-service.md) <br/> |Définit une demande de déconnexion d’un appel.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de text représente l’identificateur d’un appel.
  
## <a name="remarks"></a>Remarques

Initiale d’un appel, utilisez [l’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) ou [PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md). Utilisez la valeur de texte qui est renvoyée dans les éléments [PlayOnPhoneResponse (service web de messagerie unifiée)](playonphoneresponse-um-web-service.md) ou [PlayOnPhoneGreetingResponse (service web de messagerie unifiée)](playonphonegreetingresponse-um-web-service.md) pour la valeur de texte d’élément **CallId** . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md)
  
[(Service web de messagerie unifiée) de l’opération de déconnexion](disconnect-operation-um-web-service.md)
  
[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

