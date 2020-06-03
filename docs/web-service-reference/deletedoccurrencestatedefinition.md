---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: Le DeletedOccurrenceStateDefinition spécifie l’état d’une occurrence supprimée d’un élément de calendrier.
ms.openlocfilehash: ff8ad1d9c35d7bab3f6fe2cd1896bb16384c18e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458795"
---
# <a name="deletedoccurrencestatedefinition"></a>DeletedOccurrenceStateDefinition

Le **DeletedOccurrenceStateDefinition** spécifie l’état d’une occurrence supprimée d’un élément de calendrier. 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 **DeletedOccurrenceStateDefinitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Occurrence (transition de fuseau horaire)](occurrence-time-zone-transition.md) <br/> |Spécifie la date de l’occurrence d’un élément de calendrier.  <br/> |
|[IsOccurrencePresent](isoccurrencepresent.md) <br/> |Spécifie une valeur de type Boolean qui indique si une occurrence de l’élément de calendrier est présente.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[StateDefinition](statedefinition.md) <br/> |Spécifie une définition d’État.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

