---
title: Définition de fuseau horaire
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
description: L’élément de la définition de fuseau horaire spécifie les périodes et les transitions qui définissent un fuseau horaire.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838736"
---
# <a name="timezonedefinition"></a>Définition de fuseau horaire

L’élément de la **définition de fuseau horaire** spécifie les périodes et les transitions qui définissent un fuseau horaire. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Identificateur unique du fuseau horaire.  <br/> |
|Nom  <br/> |Représente le nom descriptif du fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Périodes](periods.md) <br/> |Représente un tableau d’éléments de [période](period.md) qui définissent le décalage de temps à différents stades du fuseau horaire.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient les transitions de fuseau horaire.  <br/> |
|[Transitions](transitions.md) <br/> |Représente un tableau des transitions de fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Représente un tableau des définitions de fuseau horaire.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Représente la définition de fuseau horaire par défaut qui doit être utilisé pour les propriétés DateTime des objets qui sont créés, mis à jour et récupérés à l’aide d’Exchange Web Services (EWS) de portée.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

