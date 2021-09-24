---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: L’élément Offset décrit le décalage par rapport à baseOffset. Avec l’élément BaseOffset, l’élément Offset identifie si l’heure est standard ou l’heure d’été.
ms.openlocfilehash: af9a2f7a94ae0cd736a4fe6f11b8a5a77673bbe3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515389"
---
# <a name="offset"></a>Offset

**L’élément Offset** décrit le décalage par rapport à [baseOffset](baseoffset.md). Avec **l’élément BaseOffset,** l’élément **Offset** identifie si l’heure est standard ou l’heure d’été. 
  
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
|[Daylight](daylight.md) <br/> |Représente la date et l’heure de passage de l’heure d’été à l’heure standard.  <br/> |
|[Standard](standard.md) <br/> |Représente la date et l’heure de passage de l’heure d’été à l’heure standard.  <br/> |
   
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

