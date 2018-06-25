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
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828243"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

L’élément **LegacyDN** identifie la boîte aux lettres d’un utilisateur par un nom unique hérité. 
  
```xml
<LegacyDN/>
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
|[Demande (POX)](request-pox.md) <br/> |Contient la demande au service de découverte automatique.  <br/> |
|[Utilisateur (POX)](user-pox.md) <br/> |Fournit des informations spécifiques à l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente l’adresse de messagerie hérités d’un utilisateur.
  
## <a name="remarks"></a>Remarques

L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est un autre élément pour une demande de découverte automatique. Il est utilisé lorsqu’une boîte aux lettres existe sur un ordinateur qui exécute Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

