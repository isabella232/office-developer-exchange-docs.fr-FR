---
title: End
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: L’élément End représente la fin d’une durée.
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456142"
---
# <a name="end"></a>End

L’élément **end** représente la fin d’une durée. 
  
```xml
<End/>
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
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Réunions](occurrence.md) <br/> |Représente une occurrence modifiée unique d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente la fin d’une durée.
  
## <a name="remarks"></a>Remarques

L’opération UpdateItem peut définir l’heure de [début](start.md) et de **fin** d’un élément de la banque Exchange. Dans une requête UpdateItem, vous pouvez définir l’heure de [début](start.md) sans définir également l’heure de **fin** . Cela peut entraîner une erreur si l’heure de [début](start.md) est postérieure à l’heure de **fin** . N’oubliez pas que les applications clientes doivent effectuer des ajustements à l’heure de **fin** lorsque cette heure de [début](start.md) est modifiée afin de conserver la durée. 
  
 **Note** Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de **fin** de l’élément de gabarit périodique n’ont pas de date égale à la première occurrence d’une périodicité hebdomadaire. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[WeeklyRecurrence](weeklyrecurrence.md)
  
 **End**


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

