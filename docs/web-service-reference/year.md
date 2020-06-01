---
title: Year
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: L’élément Year est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: cc83f9b2137f151f3f8ef0ceaf603ec036989961
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465169"
---
# <a name="year"></a>Year

L’élément **year** est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<Year/>
```

**chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StandardTime Element](standardtime.md) <br/> |Représente un décalage entre l’heure par rapport à l’heure UTC (Coordinated Universal Time) représentée par l’élément [bias (UTC)](bias-utc.md) .  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Représente un décalage entre l’heure par rapport à l’heure UTC (Coordinated Universal Time) représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.  <br/> |
   
## <a name="text-value"></a>Valeur texte

L’élément Year accepte une chaîne qui représente une année. Le format de l’année est YYYY.
  
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

