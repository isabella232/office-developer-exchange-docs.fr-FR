---
title: Statut (service web de messagerie unifiée - SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: L’élément Status définit la valeur à utiliser dans une demande d’opération SetOofStatus (service web de um).
ms.openlocfilehash: fc4806e4978ae51ec6113ff8fd45da7db223a071
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546937"
---
# <a name="status-um-web-service---setoofstatus"></a>Statut (service web de messagerie unifiée - SetOofStatus)

**L’élément Status** définit la valeur à utiliser dans une demande d’opération [SetOofStatus (service web de um).](setoofstatus-operation-um-web-service.md) 
  
[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[Statut (service web de messagerie unifiée - SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
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
|[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md) <br/> |Définit une demande de définition de l’état d’absence du Office de messagerie unifiée pour l’utilisateur qui effectue la demande.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur boolé américaine est requise. Les valeurs possibles sont les suivantes :
  
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



[Opération SetOofStatus (service web de messagerie unifiée)](setoofstatus-operation-um-web-service.md)

