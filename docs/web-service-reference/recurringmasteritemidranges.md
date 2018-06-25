---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: L’élément RecurringMasterItemIdRanges spécifie un tableau de plages d’occurrences.
ms.openlocfilehash: 60d987f475bed5d630a1238550e4d14578ebd0d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829016"
---
# <a name="recurringmasteritemidranges"></a>RecurringMasterItemIdRanges

L’élément **RecurringMasterItemIdRanges** spécifie un tableau de plages d’occurrences. 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 **RecurringMasterItemIdRangesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |La valeur de texte de l’attribut **Id** est l’identificateur unique d’un rendez-vous périodique. Il s’agit d’une valeur de **type string** .  <br/> |
|**ChangeKey** <br/> |La valeur de texte de l’attribut **ChangeKey** est modifier la clé de l’élément maître périodique. Il s’agit d’une valeur de **type string** .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[Plages](ranges.md)
  
### <a name="parent-elements"></a>Éléments parents

[ItemId](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [les GroupID](groupids.md)
  
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
   

