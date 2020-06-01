---
title: PlayOnPhoneResponse (service Web de messagerie unifiée)
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
description: L’élément PlayOnPhoneResponse définit une réponse à une opération PlayOnPhone (service Web de messagerie unifiée).
ms.openlocfilehash: ddb9cc9a8feaeb476e6502339fdc74d024797b9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459615"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (service Web de messagerie unifiée)

L’élément **PlayOnPhoneResponse** définit une réponse à une [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) . 
  
[PlayOnPhoneResponse (service Web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
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

Une valeur de texte est requise. La valeur de texte est l’identificateur d’appel à utiliser pour la valeur de [CallId (service Web de messagerie unifiée)](callid-um-web-service.md) dans une demande [GetCallInfo Operation (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) ou une [opération de déconnexion (service Web de messagerie unifiée](disconnect-operation-um-web-service.md) ). 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md)

