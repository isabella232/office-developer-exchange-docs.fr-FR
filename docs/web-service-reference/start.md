---
title: Début
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: L’élément Start représente le début d’une durée.
ms.openlocfilehash: 7342e285e57a165ec4a9ba0b8551bfbe045d3b9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521269"
---
# <a name="start"></a>Début

**L’élément Start** représente le début d’une durée. 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Représente une occurrence supprimée d’un élément de calendrier périodique.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une occurrence modifiée unique d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le début d’une durée.
  
## <a name="remarks"></a>Remarques

L’opération UpdateItem peut [](end-ex15websvcsotherref.md) définir l’heure [de](start.md) début et de fin d’un Exchange magasin. Dans une demande UpdateItem, l’heure **de** début peut être définie sans définir l’heure **de** fin. Cela peut provoquer une erreur si l’heure **de** début est ultérieure à **l’heure de** fin. N’ignorez pas que les  applications clientes doivent effectuer des ajustements à l’heure de fin lorsque cette heure de début est modifiée afin de conserver la durée.  
  
> [!NOTE]
> Les informations de décalage de [](start.md) fuseau horaire sont perdues si les [dates](end-ex15websvcsotherref.md) de début et de fin de l’élément principal périodique ne sont pas égales à la première occurrence d’une fréquence hebdomadaire de récurrence. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

