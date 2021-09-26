---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: L’élément AbsoluteMonthlyRecurrence représente une périodité mensuelle.
ms.openlocfilehash: 7fcc1811a7c42fc653344fb3c052adac820d6a5d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546916"
---
# <a name="absolutemonthlyrecurrence"></a>AbsoluteMonthlyRecurrence

**L’élément AbsoluteMonthlyRecurrence** représente une périodité mensuelle. 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 **AbsoluteMonthlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DayOfMonth](dayofmonth.md) <br/> |Décrit le jour d’un mois où un élément périodique se produit. La plage de valeurs de cette propriété est de 1 à 31. Si, pour un mois particulier, cette valeur est supérieure au nombre de jours du mois, le dernier jour du mois est supposé pour cette propriété.  <br/> |
|[Interval](interval.md) <br/> |Définit l’intervalle entre deux éléments périodiques consécutifs. Par exemple, si la valeur de **l’élément Interval** est 5, l’élément périodique se produit tous les 5 mois. La plage de valeurs valides est de 1 à 99.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de récurrence pour les tâches périodiques.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la tendance de récurrence des éléments de calendrier et des demandes de réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

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

