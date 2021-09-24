---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: L’élément RedirectUrl contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé et qui doit être utilisé pour obtenir les paramètres de découverte automatique.
ms.openlocfilehash: d515f3f79f2370dc496614bab0a3f77300ad4e30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513527"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

**L’élément RedirectUrl** contient l’URL de l’ordinateur exécutant Microsoft Exchange Server 2007 sur le rôle serveur d’accès au client qui doit être utilisé pour obtenir les paramètres de découverte automatique. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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
|[Account (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’URL du serveur d’accès au client qui doit être utilisée pour obtenir les paramètres de découverte automatique.
  
## <a name="remarks"></a>Remarques

L’application cliente doit arrêter la redirection après 10 redirections.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

