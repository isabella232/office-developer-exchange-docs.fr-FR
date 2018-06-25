---
title: Action
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: L’élément To spécifie la cible de la transition de fuseau horaire. La cible est une période de fuseau horaire ou un groupe des transitions de fuseau horaire.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838730"
---
# <a name="to"></a>Action

L’élément **To** spécifie la cible de la transition de fuseau horaire. La cible est une période de fuseau horaire ou un groupe des transitions de fuseau horaire. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Type  <br/> |Indique si la cible de transition de fuseau horaire est une période de fuseau horaire ou d’un groupe de transitions de fuseau horaire.  <br/> |
   
#### <a name="kind-attribute-values"></a>Valeurs d’attribut de type

|**Valeur**|**Description**|
|:-----|:-----|
|Point  <br/> |Spécifie que la cible de transition de fuseau horaire est une période de fuseau horaire.  <br/> |
|Groupe  <br/> |Spécifie que la cible de transition de fuseau horaire est un groupe de transitions de fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Représente une transition de fuseau horaire qui se produit à une date spécifique, à un moment spécifique.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Représente une transition de fuseau horaire qui se produit sur un jour spécifié de l’année.  <br/> |
|[Transition](transition.md) <br/> |Représente une transition de fuseau horaire.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est une chaîne qui spécifie l’identificateur unique de la [période](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire. 
  
## <a name="remarks"></a>Remarques

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

