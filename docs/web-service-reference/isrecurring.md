---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: L’élément IsRecurring indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique. Cet élément est en lecture seule.
ms.openlocfilehash: 72c71c1955b69f1c0df855ce4bd0ed02d4c89122
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526486"
---
# <a name="isrecurring"></a>IsRecurring

L’élément **IsRecurring** indique si un élément de calendrier, une demande de réunion ou une tâche fait partie d’un élément périodique. Cet élément est en lecture seule. 
  
```xml
<IsRecurring/>
```

 **Boolean**
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
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur Boolean est requise.
  
## <a name="remarks"></a>Remarques

Le tableau suivant montre comment la propriété **IsRecurring** est définie pour différents types d’éléments de calendrier pour les organisateurs et les participants, ainsi que pour les demandes de réunion et les mises à jour. 
  
|**Type CalendarItem**|**Organisateur <br/> (IsRecurring)**|**Participant <br/> (IsRecurring)**|**Demande de réunion/mise à jour <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Occurrence unique  <br/> |**TRUE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
|Masque périodique  <br/> |**TRUE** <br/> |**A** <br/> |**A** <br/> |
|Exception périodique  <br/> |**A** <br/> |**A** <br/> |**A** <br/> |
   
La valeur de la propriété **IsRecurring** définie pour les éléments de calendrier principal périodique de l’organisateur est incorrecte ; Cette valeur doit être définie sur **true**. 
  
> [!NOTE]
> L’opération GetUserAvailability a également un élément [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[TaskType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

