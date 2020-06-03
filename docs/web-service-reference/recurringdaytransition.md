---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: L’élément RecurringDayTransition représente une transition de fuseau horaire qui se produit chaque année le même jour.
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468466"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

L’élément **RecurringDayTransition** représente une transition de fuseau horaire qui se produit chaque année le même jour. 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 **RecurringDayTransitionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[To](to.md) <br/> |Spécifie le [point](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Représente le décalage de durée par rapport au temps universel coordonné (UTC) pour la transition de fuseau horaire.  <br/> |
|[Mois (transition de fuseau horaire)](month-time-zone-transition.md) <br/> |Représente le mois au cours duquel la transition de fuseau horaire a lieu.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Représente le jour de la semaine où la transition de fuseau horaire a lieu.  <br/> |
|[Occurrence (transition de fuseau horaire)](occurrence-time-zone-transition.md) <br/> |Représente l’occurrence du jour de la semaine du mois où la transition de fuseau horaire se produit.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Un exemple de transition de fuseau horaire qui pourrait être représentée par l’élément [RecurringDayTransition](recurringdaytransition.md) est une transition qui a lieu le deuxième mardi de février chaque année. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

