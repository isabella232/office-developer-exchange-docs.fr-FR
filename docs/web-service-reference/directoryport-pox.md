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
description: L’élément DirectoryPort Spécifie le port utilisé pour se connecter au répertoire lorsque le protocole fournisseur Interface NSPI (Name Service) est utilisé.
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755935"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

L’élément **DirectoryPort** Spécifie le port utilisé pour se connecter au répertoire lorsque le protocole fournisseur Interface NSPI (Name Service) est utilisé. 
  
- [Découverte automatique (POX)](autodiscover-pox.md) 
- [Réponse (POX)](response-pox.md)  
- [Compte (POX)](account-pox.md)  
- [Protocole (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
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

La valeur de texte représente le port utilisé pour accéder au serveur Exchange.
  
## <a name="remarks"></a>Remarques

L’élément **DirectoryPort** est uniquement utilisé lorsque l’élément de [Type (POX)](type-pox.md) est égale à EXCH ou EXPR. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

