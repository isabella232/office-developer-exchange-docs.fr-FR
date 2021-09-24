---
title: Year
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: L’élément Year est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 80b4ce642a7a08631140e583fb9d92143f485ea3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509279"
---
# <a name="year"></a>Year

**L’élément Year** est utilisé pour définir un fuseau horaire qui change en fonction de l’année. Cet élément est facultatif. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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
|[StandardTime](standardtime.md) <br/> |Représente un décalage par rapport à l’heure par rapport au temps universel coordonné (UTC) représenté par l’élément [Bias (UTC).](bias-utc.md)  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Représente un décalage par rapport à l’heure UTC (Coordinated Universal Time) qui est représenté par l’élément [Bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.  <br/> |
   
## <a name="text-value"></a>Valeur texte

L’élément Year accepte une chaîne qui représente une année. Le format de l’année est AAA.
  
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

