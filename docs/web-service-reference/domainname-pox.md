---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: L’élément DomainName spécifie le domaine de l’utilisateur.
ms.openlocfilehash: 9242c867d684bf9803f8c6ed1082d578cca05505
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526432"
---
# <a name="domainname-pox"></a>DomainName (POX)

**L’élément DomainName** spécifie le domaine de l’utilisateur. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [DomainName (POX)](domainname-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte spécifie le domaine de l’utilisateur.
  
## <a name="remarks"></a>Remarques

Si aucune valeur n’est spécifiée, l’authentification par défaut consiste à utiliser l’adresse de messagerie en tant que format de nom d’utilisateur principal (UPN). Par exemple : \<Username\> @ \<Domain\> .
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

