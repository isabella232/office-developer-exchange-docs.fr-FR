---
title: Time (TimeChangeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Time
api_type:
- schema
ms.assetid: be12e41e-6871-4f6b-b2d4-3dfa404f9ea1
description: L’élément Time décrit l’heure à quel moment l’heure change entre l’heure standard et l’heure d’été.
ms.openlocfilehash: 0c669340778496958ef6dff082e48b5b7f6209b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523306"
---
# <a name="time-timechangetype"></a>Time (TimeChangeType)

**L’élément Time** décrit l’heure à quel moment l’heure change entre l’heure standard et l’heure d’été. 
  
```xml
<Time/>
```

 **Time**
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

La valeur de texte représente l’heure à quel moment l’heure change entre l’heure standard et l’heure d’été.
  
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

