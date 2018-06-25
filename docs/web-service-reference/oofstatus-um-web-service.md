---
title: OofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: L’élément OofStatus contient une valeur que l’état Unified Messaging d’absence du bureau de l’utilisateur qui effectue une demande de (service web de messagerie unifiée) opération GetUMProperties indicaties.
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828650"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (service web de messagerie unifiée)

L’élément **OofStatus** contient une valeur qui indicaties l’état Unified Messaging d’absence du bureau de l’utilisateur qui effectue une demande [d’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (service web de messagerie unifiée)](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md) <br/> |Définit une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de type Boolean texte est requise. Les valeurs possibles sont les suivantes :
  
- True
    
- Faux
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)

