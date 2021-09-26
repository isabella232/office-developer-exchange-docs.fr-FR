---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: L’élément DeploymentId identifie de manière unique Microsoft Exchange Server forêt 2007.
ms.openlocfilehash: 37d66eadb38f02e75a35d0516b36aff07dfdafa6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545355"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

**L’élément DeploymentId** identifie de manière unique Microsoft Exchange Server forêt 2007. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [User (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[User (POX)](user-pox.md) <br/> |Fournit des informations spécifiques à l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte identifie de manière unique la forêt Exchange 2007 au format GUID.
  
## <a name="remarks"></a>Remarques

Si vous désinstallez puis réinstallez Exchange 2007 et que vous utilisez le même nom de serveur, la valeur **DeploymentId** change. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

