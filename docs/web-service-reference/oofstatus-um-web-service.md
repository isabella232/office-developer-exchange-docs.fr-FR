---
title: OofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: L’élément OofStatus contient une valeur qui indique l’état de la messagerie unifiée hors Office pour l’utilisateur qui fait une demande d’opération GetUMProperties (service web de messagerie unifiée).
ms.openlocfilehash: 4e899317defdb4ac4c27c3fdc17d7b7222dff6a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539268"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (service web de messagerie unifiée)

**L’élément OofStatus** contient une valeur qui indique l’état de la messagerie unifiée hors Office pour l’utilisateur qui fait une demande d’opération [GetUMProperties (service web](getumproperties-operation-um-web-service.md) de messagerie unifiée). 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md) <br/> |Définit une réponse à une [demande d’opération GetUMProperties (service web de um).](getumproperties-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte boolén est requise. Les valeurs possibles sont les suivantes :
  
- Vrai
    
- Faux
    
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)

