---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: L’élément DomainRequired indique si le domaine est requis pour l’authentification.
ms.openlocfilehash: 906c99ff7a8428404ee6045b749cdb0afed882b7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540061"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

**L’élément DomainRequired indique** si le domaine est requis pour l’authentification. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md)  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte indique si le domaine est requis pour l’authentification. Les valeurs possibles sont **en cours** et **hors.** Si la valeur est **sur**, la demande suivante doit contenir le domaine du compte de l’utilisateur.
  
## <a name="remarks"></a>Remarques

Si le domaine n’est pas spécifié dans l’élément [LoginName (POX)](loginname-pox.md) ou si l’élément **LoginName** n’a pas été spécifié, l’utilisateur doit entrer le domaine pour que l’authentification réussisse. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

