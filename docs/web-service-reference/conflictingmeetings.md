---
title: ConflictingMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetings
api_type:
- schema
ms.assetid: cfff7a11-7b3a-4995-9815-afedd45ebb0f
description: L’élément ConflictingMeetings identifie tous les éléments de calendrier qui entre en conflit avec une heure de réunion.
ms.openlocfilehash: 1d2558dba41ec3e7ae2711bb2dc26f54cada827a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755538"
---
# <a name="conflictingmeetings"></a>ConflictingMeetings

L’élément **ConflictingMeetings** identifie tous les éléments de calendrier qui entre en conflit avec une heure de réunion. 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 **NonEmptyArrayOfAllItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Si cet élément est utilisé, il doit contenir un ou plusieurs éléments enfants.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
> [!NOTE]
> Bien que les éléments enfants supplémentaires sont valides par rapport au schéma, l’élément [CalendarItem](calendaritem.md) est le seul élément enfant renvoyant des Exchange Web Services (EWS) dans l’élément **ConflictingMeetings** . Cette rubrique ne répertorie pas les éléments enfants sont valides par rapport au schéma, mais ne sont pas renvoyés par EWS. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

