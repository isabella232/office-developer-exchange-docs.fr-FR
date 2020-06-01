---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: L’élément DomainRequired indique si le domaine est requis pour l’authentification.
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461323"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

L’élément **DomainRequired** indique si le domaine est requis pour l’authentification. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)  
- [Réponse (POX)](response-pox.md) 
- [Compte (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur Text indique si le domaine est requis pour l’authentification. Les valeurs possibles sont **on** et **off**. Si la valeur est **activée**, la demande suivante doit contenir le domaine du compte de l’utilisateur.
  
## <a name="remarks"></a>Remarques

Si le domaine n’est pas spécifié dans l’élément [LoginName (POX)](loginname-pox.md) ou si l’élément **LoginName** n’a pas été spécifié, l’utilisateur doit entrer le domaine pour que l’authentification réussisse. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

