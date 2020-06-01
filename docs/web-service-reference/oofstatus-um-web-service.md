---
title: OofStatus (service Web de messagerie unifiée)
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
description: L’élément OofStatus contient une valeur qui indicaties l’état de la messagerie unifiée pour l’utilisateur qui effectue une opération GetUMProperties (service Web de messagerie unifiée).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460574"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (service Web de messagerie unifiée)

L’élément **OofStatus** contient une valeur qui indicaties l’état de la messagerie unifiée pour l’utilisateur qui effectue une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (service Web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (service Web de messagerie unifiée)](oofstatus-um-web-service.md)
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUMPropertiesResponse (service Web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md) <br/> |Définit une réponse à une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte Boolean est requise. Les valeurs possibles sont les suivantes :
  
- Vrai
    
- Faux
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (service Web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)

