---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: L’élément LegacyDN identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526381"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

L’élément **LegacyDN** identifie la boîte aux lettres d’un utilisateur par un nom unique hérité. 
  
```xml
<LegacyDN/>
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
|[Demande (POX)](request-pox.md) <br/> |Contient la demande au service de découverte automatique.  <br/> |
|[Utilisateur (POX)](user-pox.md) <br/> |Fournit des informations spécifiques à l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente l’adresse de messagerie héritée d’un utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est un élément de remplacement pour une demande de découverte automatique. Il est utilisé lorsqu’une boîte aux lettres existe sur un ordinateur qui exécute Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

