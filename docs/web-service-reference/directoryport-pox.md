---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: L’élément DirectoryPort spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462086"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

L’élément **DirectoryPort** spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé. 
  
- [Découverte automatique (POX)](autodiscover-pox.md) 
- [Réponse (POX)](response-pox.md)  
- [Compte (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
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

La valeur de texte représente le port utilisé pour accéder au serveur Exchange.
  
## <a name="remarks"></a>Remarques

L’élément **DirectoryPort** est utilisé uniquement lorsque l’élément [type (POX)](type-pox.md) est égal à Exch ou Expr. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

