---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: L’élément TimeOffset représente le décalage du temps universel coordonné (UTC) pour la transition de fuseau horaire.
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838701"
---
# <a name="timeoffset"></a>TimeOffset

L’élément **TimeOffset** représente le décalage du temps universel coordonné (UTC) pour la transition de fuseau horaire. 
  
```XML
<TimeOffset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Représente une transition de fuseau horaire qui se produit à une date spécifique chaque année.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **TimeOffset** est une durée qui spécifie le décalage de l’heure UTC pour la transition de fuseau horaire. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

