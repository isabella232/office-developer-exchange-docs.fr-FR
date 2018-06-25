---
title: NumberedRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberedRecurrence
api_type:
- schema
ms.assetid: 53746909-ef21-4764-8715-a7769b943cca
description: L’élément NumberedRecurrence décrit la date de début et le nombre d’occurrences d’un élément périodique.
ms.openlocfilehash: 01fbf831fa7ff378221d4db3d873af730ac564d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828628"
---
# <a name="numberedrecurrence"></a>NumberedRecurrence

L’élément **NumberedRecurrence** décrit la date de début et le nombre d’occurrences d’un élément périodique. 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 **NumberedRecurrenceRangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartDate (périodicité)](startdate-recurrence.md) <br/> |Représente la date de début d’une tâche périodique ou d’un élément de calendrier.  <br/> |
|[NumberOfOccurrences](numberofoccurrences.md) <br/> |Contient le nombre d’occurrences d’un élément périodique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Périodicité (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contient la périodicité pour les éléments de calendrier et les demandes de réunion.  <br/> |
|[Périodicité (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contient des informations de périodicité pour les tâches répétitives.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

