---
title: État (service web de messagerie unifiée - SetOofStatus)
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
description: L’élément Status définit la valeur à utiliser dans une requête (service web de messagerie unifiée) d’opération SetOofStatus.
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829583"
---
# <a name="status-um-web-service---setoofstatus"></a>État (service web de messagerie unifiée - SetOofStatus)

L’élément **Status** définit la valeur à utiliser dans une requête [d’opération SetOofStatus (service web de messagerie unifiée)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[État (service web de messagerie unifiée - SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md) <br/> |Définit une demande pour définir l’état Unified Messaging d’absence du bureau Office (OOF) de l’utilisateur qui effectue la demande.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur booléenne est requise. Les valeurs possibles sont les suivantes :
  
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



[Opération SetOofStatus (service web de messagerie unifiée)](setoofstatus-operation-um-web-service.md)

