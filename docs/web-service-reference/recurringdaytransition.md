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
description: L’élément RecurringDayTransition représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829012"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

L’élément **RecurringDayTransition** représente une transition de fuseau horaire qui se produit sur le même jour tous les ans. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Pour](to.md) <br/> |Spécifie la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Représente le décalage de la durée du temps universel coordonné (UTC) pour la transition de fuseau horaire.  <br/> |
|[Mois (Transition fuseau horaire)](month-time-zone-transition.md) <br/> |Représente le mois dans laquelle se produit la transition de fuseau horaire.  <br/> |
|[DayOfWeek (fuseau horaire)](dayofweek-timezone.md) <br/> |Représente le jour de la semaine sur lequel se produit la transition de fuseau horaire.  <br/> |
|[Occurrence (Transition fuseau horaire)](occurrence-time-zone-transition.md) <br/> |Représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Représente une collection des transitions de fuseau horaire.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Représente une collection des transitions de fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Un exemple d’une transition de fuseau horaire qui peut être représenté par l’élément [RecurringDayTransition](recurringdaytransition.md) est une transition se produit le deuxième mardi du mois de février de chaque année. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

