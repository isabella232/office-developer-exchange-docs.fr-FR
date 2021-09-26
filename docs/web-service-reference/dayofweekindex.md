---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: L’élément DayOfWeekIndex décrit la semaine d’un mois utilisée dans une récurrence relative.
ms.openlocfilehash: 3b9af396bbd5c51b365da6a95b40b00718d47c3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542518"
---
# <a name="dayofweekindex"></a>DayOfWeekIndex

**L’élément DayOfWeekIndex** décrit la semaine d’un mois utilisée dans une récurrence relative. 
  
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
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une récurrence relative de l’année.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit une récurrence mensuelle relative.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- Premier    
- Deuxième    
- Troisième    
- Quatrième    
- Nom
    
## <a name="remarks"></a>Remarques

Par exemple, le deuxième lundi d’un mois peut se produire dans la troisième semaine de ce mois. Si un mois commence le vendredi, la première semaine du mois ne contient que quelques jours et ne contient pas de lundi. Par conséquent, le premier lundi doit avoir lieu dans la deuxième semaine.
  
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

