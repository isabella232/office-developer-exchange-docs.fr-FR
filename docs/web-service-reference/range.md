---
title: Plage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: L’élément Range spécifie une plage d’occurrences d’éléments de calendrier pour un élément de calendrier répétitif.
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465309"
---
# <a name="range"></a>Plage

L’élément **Range** spécifie une plage d’occurrences d’éléments de calendrier pour un élément de calendrier répétitif. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Start** <br/> |La valeur de texte de l’attribut **Start** est la date de début de la plage d’éléments périodiques. Il s’agit d’une valeur **DateTime** .  <br/> |
|**End** <br/> |La valeur de texte de l’attribut **end** est la date de fin de la plage d’éléments périodiques. Il s’agit d’une valeur **DateTime** .  <br/> |
|**Count** <br/> |La valeur de l’attribut **Count** est le nombre d’occurrences de l’élément périodique. Il s’agit d’une valeur **entière** .  <br/> |
|**CompareOriginalStartTime** <br/> |La valeur de texte **true** pour l’attribut **CompareOriginalStartTime** indique que le client doit comparer l’heure de début d’origine et la nouvelle heure de début. La valeur **false** indique que le client n’a pas besoin de comparer l’heure de début d’origine avec la nouvelle heure de début.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Ranges](ranges.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

