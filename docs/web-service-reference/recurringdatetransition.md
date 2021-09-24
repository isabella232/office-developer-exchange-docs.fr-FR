---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: L’élément RecurringDateTransition représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.
ms.openlocfilehash: 864f3f539c5440fbfc539ca6c2042b3d9edca267
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529362"
---
# <a name="recurringdatetransition"></a>RecurringDateTransition

**L’élément RecurringDateTransition** représente une transition de fuseau horaire qui se produit à une date spécifique chaque année. 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 **RecurringDateTransitionType**
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
|[Day](day.md) <br/> |Représente le jour du mois au cours duquel la transition de fuseau horaire a lieu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Un exemple de transition de fuseau horaire qui pourrait être représentée par l’élément [RecurringDateTransition](recurringdatetransition.md) est une transition qui se produit le 15 mars de chaque année. 
  
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

