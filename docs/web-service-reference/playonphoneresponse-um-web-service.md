---
title: PlayOnPhoneResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: L’élément PlayOnPhoneResponse définit une réponse à une demande de (service web de messagerie unifiée) opération PlayOnPhone.
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828832"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (service web de messagerie unifiée)

L’élément **PlayOnPhoneResponse** définit une réponse à une demande de [l’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) . 
  
[PlayOnPhoneResponse (service web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de text est l’identificateur d’appel à utiliser pour la valeur de [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md) dans une requête [d’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) ou une [opération de déconnexion (service web de messagerie unifiée)](disconnect-operation-um-web-service.md) . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)

