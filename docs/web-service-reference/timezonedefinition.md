---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: L’élément TimeZoneDefinition spécifie les points et les transitions qui définissent un fuseau horaire.
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466065"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

L’élément **TimeZoneDefinition** spécifie les points et les transitions qui définissent un fuseau horaire. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Représente l’identificateur unique du fuseau horaire.  <br/> |
|Nom  <br/> |Représente le nom descriptif du fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Représente un tableau d’éléments [period](period.md) qui définissent le décalage temporel à différentes étapes du fuseau horaire.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient des transitions de fuseau horaire.  <br/> |
|[Transitions](transitions.md) <br/> |Représente un tableau de transitions de fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Représente un tableau de définitions de fuseau horaire.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Représente la définition de fuseau horaire par défaut qui doit être utilisée pour la portée des propriétés DateTime des objets créés, mis à jour et récupérés à l’aide des services Web Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

