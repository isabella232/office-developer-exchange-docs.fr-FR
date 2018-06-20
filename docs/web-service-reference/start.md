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
description: L’élément de début représente le début d’une durée.
ms.openlocfilehash: 8d013990e650b497abfa947938a69eed3fed7474
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829545"
---
# <a name="start"></a>Démarrer

L’élément **Démarrer** représente le début d’une durée. 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Représente une occurrence d’un élément de calendrier périodique supprimée.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une seule occurrence de modification d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le début d’une durée.
  
## <a name="remarks"></a>Remarques

L’opération UpdateItem peut définir l’heure de [début](start.md) et [fin](end-ex15websvcsotherref.md) d’un élément de la banque Exchange. Dans une demande UpdateItem, l’heure de **début** peut être défini sans également définir l’heure de **fin** . Cela peut provoquer une erreur si l’heure de **début** est postérieure à l’heure de **fin** . Sachez que les applications clientes doivent exécuter à l’heure de **fin** lorsque que l’heure de **début** est modifiée afin de conserver la durée de corrections. 
  
> [!NOTE]
> Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de [fin](end-ex15websvcsotherref.md) de l’élément périodique principal n’ont pas de date qui est égale à la première occurrence d’une périodicité hebdomadaire. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

