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
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756030"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

L’élément **DomainRequired** indique si le domaine est requis pour l’authentification. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)  
- [Réponse (POX)](response-pox.md) 
- [Compte (POX)](account-pox.md)  
- [Protocole (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte indique si le domaine est requis pour l’authentification. Les valeurs possibles sont **on** et **off**. Si la valeur est **activée**, la requête suivante doit contenir le domaine du compte de l’utilisateur.
  
## <a name="remarks"></a>Remarques

Si le domaine n’est pas spécifié dans l’élément [LoginName (POX)](loginname-pox.md) ou l’élément **LoginName** n’a pas été spécifié, l’utilisateur doit entrer le domaine avant l’authentification réussit. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

