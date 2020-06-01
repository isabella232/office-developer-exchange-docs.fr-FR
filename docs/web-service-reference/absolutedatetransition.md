---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: L’élément AbsoluteDateTransition représente une transition de fuseau horaire qui se produit à une date spécifique et à un moment donné.
ms.openlocfilehash: 514464f69c3be5496aedbe184848ef9ed9f296b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461722"
---
# <a name="absolutedatetransition"></a>AbsoluteDateTransition

L’élément **AbsoluteDateTransition** représente une transition de fuseau horaire qui se produit à une date spécifique et à un moment donné. 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

**AbsoluteDateTransitionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[To](to.md) <br/> |Spécifie le [point](period.md) ou [TransitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire.  <br/> |
|[DateTime](datetime.md) <br/> |Représente la date et l’heure auxquelles la transition de fuseau horaire a lieu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Représente une collection de transitions de fuseau horaire.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

