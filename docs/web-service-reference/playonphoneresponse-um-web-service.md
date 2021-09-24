---
title: PlayOnPhoneResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: L’élément PlayOnPhoneResponse définit une réponse à une demande d’opération PlayOnPhone (service web de um).
ms.openlocfilehash: 9c2893837a1bc9c4836dc3cab6fb14e0d1fd611b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516523"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (service web de messagerie unifiée)

**L’élément PlayOnPhoneResponse** définit une réponse à une demande d’opération [PlayOnPhone (service web de um).](playonphone-operation-um-web-service.md) 
  
[PlayOnPhoneResponse (service web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur textuelle est l’identificateur d’appel à utiliser pour la valeur [de CallId (service web](callid-um-web-service.md) de messagerie unique) dans une demande d’opération [GetCallInfo (service web](getcallinfo-operation-um-web-service.md) de messagerie unique) ou une demande d’opération de déconnexion [(service web](disconnect-operation-um-web-service.md) de messagerie un peu plus). 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)

