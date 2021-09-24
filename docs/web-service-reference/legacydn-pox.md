---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: L’élément LegacyDN identifie la boîte aux lettres d’un utilisateur par son nom hérité.
ms.openlocfilehash: bd65e18daf1b05f66ebd767635cbe6a3135f1abf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540831"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

**L’élément LegacyDN** identifie la boîte aux lettres d’un utilisateur par son nom hérité. 
  
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
|[Request (POX)](request-pox.md) <br/> |Contient la demande au service de découverte automatique.  <br/> |
|[User (POX)](user-pox.md) <br/> |Fournit des informations spécifiques à l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’adresse de messagerie héritée d’un utilisateur.
  
## <a name="remarks"></a>Remarques

[L’élément EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est un autre élément pour une demande de découverte automatique. Il est utilisé lorsqu’une boîte aux lettres existe sur un ordinateur qui exécute Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

