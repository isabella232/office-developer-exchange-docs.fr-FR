---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: L’élément DeploymentId identifie de manière unique la forêt Microsoft Exchange Server 2007.
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755895"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

L’élément **DeploymentId** identifie de manière unique la forêt Microsoft Exchange Server 2007. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)  
- [Réponse (POX)](response-pox.md) 
- [Utilisateur (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur (POX)](user-pox.md) <br/> |Fournit des informations spécifiques à l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte identifie de manière unique la forêt Exchange 2007 au format GUID.
  
## <a name="remarks"></a>Remarques

Si vous désinstallez et réinstallez Exchange 2007 et que vous utilisez le même nom de serveur, la valeur de **DeploymentId** est modifiée. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

