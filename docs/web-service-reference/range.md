---
title: Plage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: L’élément de plage Spécifie une plage d’occurrences d’élément de calendrier pour un élément de calendrier périodique.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828946"
---
# <a name="range"></a>Plage

L’élément de **plage** spécifie une plage d’occurrences d’élément de calendrier pour un élément de calendrier périodique. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Début** <br/> |La valeur de texte de l’attribut **Démarrer** est la date de début de la plage d’éléments périodiques. Il s’agit d’une valeur **dateTime** .  <br/> |
|**End** <br/> |La valeur de texte de l’attribut de **fin** est la date de fin de la plage d’éléments périodiques. Il s’agit d’une valeur **dateTime** .  <br/> |
|**Count** <br/> |La valeur de texte de l’attribut de **nombre** est le nombre d’occurrences de l’élément périodique. Il s’agit d’une valeur **entière** .  <br/> |
|**CompareOriginalStartTime** <br/> |La valeur de texte de **la valeur true** pour l’attribut **CompareOriginalStartTime** indique que le client doit comparer l’heure de début d’origine avec la nouvelle heure de début. La valeur **false** indique que le client n’a pas besoin comparer l’heure de début d’origine avec la nouvelle heure de début.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Plages](ranges.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

