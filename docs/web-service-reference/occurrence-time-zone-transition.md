---
title: Occurrence (transition de fuseau horaire)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: L’élément Occurrence représente l’occurrence du jour de la semaine du mois où se produit la transition de fuseau horaire.
ms.openlocfilehash: 9790b0e9541da0c22f2eac59850b8a361645c7b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539276"
---
# <a name="occurrence-time-zone-transition"></a>Occurrence (transition de fuseau horaire)

**L’élément Occurrence** représente l’occurrence du jour de la semaine du mois où se produit la transition de fuseau horaire. 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit le même jour chaque année.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est un nombre complet qui représente l’occurrence du jour de la semaine du mois où se produit la transition de fuseau horaire. Le tableau suivant répertorie les valeurs possibles.
  
|**Valeur**|**Description**|
|:-----|:-----|
|1  <br/> |Première occurrence du jour spécifié de la semaine à partir du début du mois.  <br/> |
|2  <br/> |Deuxième occurrence du jour spécifié de la semaine à partir du début du mois.  <br/> |
|3  <br/> |Troisième occurrence du jour spécifié de la semaine à partir du début du mois.  <br/> |
|4   <br/> |Quatrième occurrence du jour spécifié de la semaine à partir du début du mois.  <br/> |
|-1  <br/> |Première occurrence du jour spécifié de la semaine à partir de la fin du mois.  <br/> |
|-2  <br/> |Deuxième occurrence du jour spécifié de la semaine à partir de la fin du mois.  <br/> |
|-3  <br/> |Troisième occurrence du jour spécifié de la semaine à partir de la fin du mois.  <br/> |
|-4  <br/> |Quatrième occurrence du jour spécifié de la semaine à partir de la fin du mois.  <br/> |
   
## <a name="remarks"></a>Remarques

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

