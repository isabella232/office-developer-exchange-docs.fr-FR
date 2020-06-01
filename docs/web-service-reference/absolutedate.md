---
title: AbsoluteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDate
api_type:
- schema
ms.assetid: 8bc59a26-6fe1-42e9-968c-69a94a3fb0ae
description: L’élément AbsoluteDate représente la date à laquelle le temps change à partir de l’heure standard ou de l’heure d’été.
ms.openlocfilehash: 1874fea02c1eeeb41522046963e1d1b2fcea645a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461729"
---
# <a name="absolutedate"></a>AbsoluteDate

L’élément **AbsoluteDate** représente la date à laquelle le temps change à partir de l’heure standard ou de l’heure d’été. 
  
```xml
<AbsoluteDate/>
```

**date**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Standard](standard.md) <br/> |Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.  <br/> |
|[Auxquelles](daylight.md) <br/> |Représente la date et l’heure auxquelles l’heure passe de l’heure standard à l’heure d’été.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte représente la date à laquelle le changement se produit entre l’heure standard et l’heure d’été.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)




