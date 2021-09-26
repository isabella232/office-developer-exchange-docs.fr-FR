---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: L’élément DirectoryPort spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.
ms.openlocfilehash: 223e82840628e19896bde196d7467622a2ad5002
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543330"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

**L’élément DirectoryPort** spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md)  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le port utilisé pour accéder au Exchange serveur.
  
## <a name="remarks"></a>Remarques

**L’élément DirectoryPort** est utilisé uniquement lorsque l’élément [Type (POX)](type-pox.md) est égal à EXCH ou EXPR. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

