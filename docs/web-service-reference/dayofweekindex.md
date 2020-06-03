---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: L’élément DayOfWeekIndex décrit quelle semaine d’un mois est utilisée dans une périodicité relative.
ms.openlocfilehash: c9235d83a944f9c8883439dd2adf190b88977f16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529209"
---
# <a name="dayofweekindex"></a>DayOfWeekIndex

L’élément **DayOfWeekIndex** décrit quelle semaine d’un mois est utilisée dans une périodicité relative. 
  
```xml
<DayOfWeekIndex/>
```

**DayOfWeekIndexType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une périodicité annuelle relative.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit une périodicité mensuelle relative.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- Premier    
- Deuxième    
- Troisième    
- Quatrième    
- Nom
    
## <a name="remarks"></a>Remarques

Par exemple, le deuxième lundi d’un mois peut se produire dans la troisième semaine de ce mois. Si un mois commence un vendredi, la première semaine du mois ne contient que quelques jours et ne contient pas de lundi. Par conséquent, le premier lundi doit se produire dans la deuxième semaine.
  
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

