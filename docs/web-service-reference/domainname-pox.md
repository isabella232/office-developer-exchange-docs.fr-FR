---
title: Nom_domaine (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: L’élément DomainName spécifie le domaine de l’utilisateur.
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458424"
---
# <a name="domainname-pox"></a>Nom_domaine (POX)

L’élément **DomainName** spécifie le domaine de l’utilisateur. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)  
- [Réponse (POX)](response-pox.md)  
- [Compte (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [Nom_domaine (POX)](domainname-pox.md)
  
```xml
<DomainName/>
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

La valeur texte spécifie le domaine de l’utilisateur.
  
## <a name="remarks"></a>Remarques

Si aucune valeur n’est spécifiée, l’authentification par défaut consiste à utiliser l’adresse de messagerie en tant que format de nom d’utilisateur principal (UPN). Par exemple : \<Username\> @ \<Domain\> .
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

