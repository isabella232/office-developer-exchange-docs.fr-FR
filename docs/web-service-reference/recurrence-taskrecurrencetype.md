---
title: Périodicité (TaskRecurrenceType)
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
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: L’élément de périodicité contient des informations de périodicité pour les tâches répétitives.
ms.openlocfilehash: ae2bb35e89a0a50c7ca67cb0e580427150afb99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829006"
---
# <a name="recurrence-taskrecurrencetype"></a>Périodicité (TaskRecurrenceType)

L’élément de **périodicité** contient des informations de périodicité pour les tâches répétitives. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 **TaskRecurrenceType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Décrit une périodicité annuelle relative d’une tâche périodique.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Représente une périodicité annuelle pour une tâche périodique.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Décrit une périodicité mensuelle relative d’une tâche périodique.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Représente une périodicité mensuelle pour une tâche périodique.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Décrit la fréquence, en semaines et les jours où une tâche est périodique.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Décrit la fréquence, en jours, dans laquelle une tâche est périodique.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Décrit le nombre de jours après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Décrit le nombre de semaines après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Décrit le nombre de mois après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Indique combien d’années après l’achèvement de la tâche en cours de la prochaine occurrence à échéance.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Décrit une périodicité qui n’a pas une date de fin définie.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [EndDateRecurrence](enddaterecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Décrit la date de début et date de fin de périodicité d’un élément.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [NumberedRecurrence](numberedrecurrence.md) .  <br/> [EndDateRecurrence](enddaterecurrence.md) ne peut pas être utilisé avec un motif de régénération.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Décrit la date de début et le nombre d’occurrences d’un élément périodique.  <br/> L’utilisation de cet élément exclut l’utilisation des éléments [NoEndRecurrence](noendrecurrence.md) et [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
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

