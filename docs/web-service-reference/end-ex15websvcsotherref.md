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
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756168"
---
# <a name="end"></a>End

L’élément **End** représente la fin d’une durée. 
  
```xml
<End/>
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
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une seule occurrence de modification d’un élément de calendrier périodique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente la fin d’une durée.
  
## <a name="remarks"></a>Remarques

L’opération UpdateItem peut définir l’heure de [début](start.md) et **fin** d’un élément de la banque Exchange. Dans une demande UpdateItem, vous pouvez définir l’heure de [début](start.md) sans également définir l’heure de **fin** . Cela peut provoquer une erreur si l’heure de [début](start.md) est postérieure à l’heure de **fin** . Sachez que les applications clientes doivent exécuter à l’heure de **fin** lorsque que l’heure de [début](start.md) est modifiée afin de conserver la durée de corrections. 
  
 **Remarque** Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de **fin** de l’élément périodique principal n’ont pas de date qui est égale à la première occurrence d’une périodicité hebdomadaire. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[WeeklyRecurrence](weeklyrecurrence.md)
  
 **End**


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

