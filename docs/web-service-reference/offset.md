---
title: Décalage
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
description: L’élément de décalage décrit le décalage de le BaseOffset. Avec l’élément BaseOffset, l’élément de décalage indique si l’heure est standard ou l’heure d’été.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828642"
---
# <a name="offset"></a>Décalage

L’élément de **décalage** décrit le décalage de l' [BaseOffset](baseoffset.md). Avec l’élément **BaseOffset** , l’élément **décalage** indique si l’heure est standard ou l’heure d’été. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Heure d’été](daylight.md) <br/> |Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.  <br/> |
|[Standard](standard.md) <br/> |Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le décalage du temps universel coordonné (UTC).
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

