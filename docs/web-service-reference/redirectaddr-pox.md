---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: L’élément RedirectAddr spécifie l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529874"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

L’élément **RedirectAddr** spécifie l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.
  
## <a name="remarks"></a>Remarques

Si cet élément est présent dans la réponse de découverte automatique, effectuez une autre demande à l’aide de la valeur de texte de l’élément **RedirectAddr** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

