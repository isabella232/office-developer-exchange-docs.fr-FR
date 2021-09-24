---
title: Plage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: L’élément Range spécifie une plage d’occurrences d’éléments de calendrier pour un élément de calendrier exexaser.
ms.openlocfilehash: 0d16dad24dda48f084b3011d7b96eb719431d9da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519099"
---
# <a name="range"></a>Plage

**L’élément Range** spécifie une plage d’occurrences d’éléments de calendrier pour un élément de calendrier exexaser. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Start** <br/> |La valeur de texte de **l’attribut Start** est la date de début de la plage d’éléments périodiques. Il s’agit **d’une valeur dateTime.**  <br/> |
|**End** <br/> |La valeur de texte de **l’attribut End** est la date de fin de la plage d’éléments périodiques. Il s’agit **d’une valeur dateTime.**  <br/> |
|**Count** <br/> |La valeur de texte de **l’attribut Count** est le nombre d’occurrences de l’élément périodique. Il s’agit **d’une valeur d’un groupe de** valeurs.  <br/> |
|**CompareOriginalStartTime** <br/> |La valeur de texte **true** pour l’attribut **CompareOriginalStartTime** indique que le client doit comparer l’heure de début d’origine avec la nouvelle heure de début. La valeur **false indique** que le client n’a pas besoin de comparer l’heure de début d’origine avec la nouvelle heure de début.  <br/> |
   
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
   

