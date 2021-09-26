---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: L’élément RecurringDayTransition représente une transition de fuseau horaire qui se produit le même jour chaque année.
ms.openlocfilehash: 3b567e5b906ec00bd71deb1c85f8049bb6de8e3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542882"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

**L’élément RecurringDayTransition** représente une transition de fuseau horaire qui se produit le même jour chaque année. 
  
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
|[To](to.md) <br/> |Spécifie la période [ou](period.md) [TransitionsGroup qui](transitionsgroup.md) est la cible de la transition de fuseau horaire.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Représente le décalage de durée par rapport au temps universel coordonné (UTC) pour la transition de fuseau horaire.  <br/> |
|[Month (transition de fuseau horaire)](month-time-zone-transition.md) <br/> |Représente le mois au cours duquel la transition de fuseau horaire a lieu.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Représente le jour de la semaine au cours duquel la transition de fuseau horaire a lieu.  <br/> |
|[Occurrence (transition de fuseau horaire)](occurrence-time-zone-transition.md) <br/> |Représente l’occurrence du jour de la semaine dans le mois où la transition de fuseau horaire se produit.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Un exemple de transition de fuseau horaire qui peut être représenté par l’élément [RecurringDayTransition](recurringdaytransition.md) est une transition qui se produit le deuxième mardi de février de chaque année. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

