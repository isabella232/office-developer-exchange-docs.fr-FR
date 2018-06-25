---
title: Occurrence (Transition fuseau horaire)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: L’élément Occurrence représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire.
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828636"
---
# <a name="occurrence-time-zone-transition"></a>Occurrence (Transition fuseau horaire)

L’élément **Occurrence** représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire. 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit sur le même jour tous les ans.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est un entier qui représente l’occurrence du jour de la semaine dans le mois qui se produit la transition de fuseau horaire. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|1  <br/> |La première occurrence du jour de la semaine à partir du début du mois spécifié.  <br/> |
|2  <br/> |La deuxième occurrence du jour de la semaine à partir du début du mois spécifié.  <br/> |
|3  <br/> |La troisième occurrence du jour de la semaine à partir du début du mois spécifié.  <br/> |
|4  <br/> |La quatrième occurrence du jour de la semaine à partir du début du mois spécifié.  <br/> |
|-1  <br/> |La première occurrence du jour de semaine à partir de la fin du mois spécifié.  <br/> |
|-2  <br/> |La deuxième occurrence du jour de semaine à partir de la fin du mois spécifié.  <br/> |
|-3  <br/> |La troisième occurrence du jour de semaine à partir de la fin du mois spécifié.  <br/> |
|-4  <br/> |La quatrième occurrence du jour de semaine à partir de la fin du mois spécifié.  <br/> |
   
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

