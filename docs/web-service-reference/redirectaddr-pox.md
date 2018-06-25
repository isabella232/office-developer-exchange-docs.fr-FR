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
description: L’élément RedirectAddr Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829020"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

L’élément **RedirectAddr** Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte pour l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de text représente l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.
  
## <a name="remarks"></a>Remarques

Si cet élément est présent dans la réponse de découverte automatique, effectuer une autre demande à l’aide de la valeur de texte de l’élément **RedirectAddr** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

