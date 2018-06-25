---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: L’élément RedirectUrl contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829027"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

L’élément **RedirectUrl** contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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

La valeur de text représente l’URL du serveur d’accès Client qui doit être utilisé pour obtenir les paramètres de découverte automatique.
  
## <a name="remarks"></a>Remarques

L’application cliente doit s’arrêter redirection après 10 redirections.
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

