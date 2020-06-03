---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: L’élément DaysOfWeek décrit les jours de la semaine utilisés dans les périodicités des éléments.
ms.openlocfilehash: 3036cbe3f93ff87b9a4d5dc7bf164e3e952b06fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463719"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

L’élément **DaysOfWeek** décrit les jours de la semaine utilisés dans les périodicités des éléments. 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit une périodicité hebdomadaire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- Warm    
- Lundi    
- Mardi    
- Mercredi    
- Jeudi    
- Vendredi    
- Samedi    
- Day (cette valeur n’est pas valide pour un modèle de périodicité hebdomadaire)    
- Weekday (cette valeur n’est pas valide pour un modèle de périodicité hebdomadaire)    
- WeekendDay (cette valeur n’est pas valide pour un modèle de périodicité hebdomadaire)
    
Un modèle de périodicité hebdomadaire peut contenir plusieurs valeurs. Les valeurs sont séparées par un espace. Par exemple, pour une périodicité hebdomadaire le mardi et le jeudi, la valeur du texte sera « mardi jeudi ».
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

