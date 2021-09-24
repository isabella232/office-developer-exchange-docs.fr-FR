---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: L’élément Reminder spécifie un rappel pour une tâche ou un élément de calendrier.
ms.openlocfilehash: 97b4a1dfb2739ff9ea335bca1e61e264715ced30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512491"
---
# <a name="reminder"></a>Reminder

**L’élément Reminder** spécifie un rappel pour une tâche ou un élément de calendrier. 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 **ReminderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Objet](subject.md)  |  [Emplacement](location.md)  |  [ReminderTime](remindertime.md)  |  [StartDate](startdate.md)  |  [EndDate (ReminderType)](enddate-remindertype.md)  |  [ItemId](itemid.md)  |  [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  [ReminderGroup](remindergroup.md)  |  [UID](uid.md)
  
### <a name="parent-elements"></a>Éléments parents

[Reminders](reminders.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Reminders](reminders.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

