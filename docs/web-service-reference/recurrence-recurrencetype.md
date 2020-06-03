---
title: Récurrence (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: L’élément Recurrence contient la périodicité des éléments de calendrier et des demandes de réunion.
ms.openlocfilehash: d00445c75fb35c3bb99eeed06e30cb1cf2883597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529888"
---
# <a name="recurrence-recurrencetype"></a>Récurrence (RecurrenceType)

L’élément **Recurrence** contient la périodicité des éléments de calendrier et des demandes de réunion. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

**RecurrenceType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une périodicité annuelle relative.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Représente une périodicité annuelle.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit un modèle de périodicité mensuelle relative pour un élément de calendrier périodique.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Représente une périodicité mensuelle.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit la fréquence, en semaines, et les jours de récurrence d’un élément de calendrier ou d’une tâche.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Décrit la fréquence, en jours, de récurrence d’une tâche ou d’un élément de calendrier.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Décrit un modèle de récurrence qui n’a pas de date de fin définie.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Décrit la date de début et la date de fin d’une périodicité d’élément.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Décrit la date de début et le nombre d’occurrences d’un élément périodique.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la Banque d’aide Exchange  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster. 
  
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

