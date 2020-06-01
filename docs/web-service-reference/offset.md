---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: L’élément offset décrit le décalage par rapport à l’BaseOffset. Avec l’élément BaseOffset, l’élément offset identifie s’il s’agit de l’heure standard ou de l’heure d’été.
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459755"
---
# <a name="offset"></a>Offset

L’élément **offset** décrit le décalage par rapport à l' [BaseOffset](baseoffset.md). Avec l’élément **BaseOffset** , l’élément **offset** identifie s’il s’agit de l’heure standard ou de l’heure d’été. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Auxquelles](daylight.md) <br/> |Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.  <br/> |
|[Standard](standard.md) <br/> |Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le décalage par rapport au temps universel coordonné (UTC).
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

