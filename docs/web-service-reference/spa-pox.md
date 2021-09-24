---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: L’élément SPA indique si l’authentification par mot de passe sécurisé (SPA) est requise.
ms.openlocfilehash: 8737a5b923d4f59c2819f7574924352223ac3673
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540411"
---
# <a name="spa-pox"></a>SPA (POX)

**L’élément SPA** indique si l’authentification par mot de passe sécurisé (SPA) est requise. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[SPA (POX)](spa-pox.md)
  
```xml
<SPA/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte indique si SPA est requis. Si la valeur de texte **est sur**, SPA est obligatoire.
  
## <a name="remarks"></a>Remarques

Si cet élément n’est pas présent, la valeur par défaut est définie sur **.**
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

