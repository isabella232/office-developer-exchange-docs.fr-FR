---
title: Démarrer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: L’élément Start représente le début d’une durée.
ms.openlocfilehash: 0daf9c1422f7ba3894f9785aacac58263c5e721e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457213"
---
# <a name="start"></a>Démarrer

L’élément **Start** représente le début d’une durée. 
  
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
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Réunions](occurrence.md) <br/> |Représente une occurrence modifiée unique d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le début d’une durée.
  
## <a name="remarks"></a>Remarques

L’opération UpdateItem peut définir l’heure de [début](start.md) et de [fin](end-ex15websvcsotherref.md) d’un élément de la banque Exchange. Dans une requête UpdateItem, l’heure de **début** peut être définie sans définir également l’heure de **fin** . Cela peut entraîner une erreur si l’heure de **début** est postérieure à l’heure de **fin** . N’oubliez pas que les applications clientes doivent effectuer des ajustements à l’heure de **fin** lorsque cette heure de **début** est modifiée afin de conserver la durée. 
  
> [!NOTE]
> Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de [fin](end-ex15websvcsotherref.md) de l’élément de gabarit périodique n’ont pas de date égale à la première occurrence d’une périodicité hebdomadaire. 
  
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

