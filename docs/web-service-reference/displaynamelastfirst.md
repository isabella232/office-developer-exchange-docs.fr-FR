---
title: DisplayNameLastFirst
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d392e138-a514-4bce-81b1-1f484e353d1c
description: L’élément DisplayNameLastFirst Spécifie le nom complet du personnage associé dans le format, nom de famille, prénom.
ms.openlocfilehash: 68ebf0e91e216cffa1ba8db425de248f0d4e77b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756009"
---
# <a name="displaynamelastfirst"></a>DisplayNameLastFirst

L’élément **DisplayNameLastFirst** Spécifie le nom complet du personnage associé au format « Nom », « Prénom ». 
  
```XML
<DisplayNameLastFirst></DisplayNameLastFirst>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Personnage](persona.md) <br/> |Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **DisplayNameLastFirst** est une valeur de type string qui spécifie le nom complet, avec le nom de famille tout d’abord. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

