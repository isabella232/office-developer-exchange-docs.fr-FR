---
title: État (service Web de messagerie unifiée-SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: L’élément Status définit la valeur à utiliser dans une demande d’opération SetOofStatus (service Web de messagerie unifiée).
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459979"
---
# <a name="status-um-web-service---setoofstatus"></a>État (service Web de messagerie unifiée-SetOofStatus)

L’élément **Status** définit la valeur à utiliser dans une demande d' [opération SetOofStatus (service Web de messagerie unifiée)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (service Web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[État (service Web de messagerie unifiée-SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (service Web de messagerie unifiée)](setoofstatus-um-web-service.md) <br/> |Définit une demande de définition de l’état d’absence du Bureau de la messagerie unifiée pour l’utilisateur qui effectue la demande.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur booléenne est requise. Les valeurs possibles sont les suivantes :
  
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



[Opération SetOofStatus (service Web de messagerie unifiée)](setoofstatus-operation-um-web-service.md)

