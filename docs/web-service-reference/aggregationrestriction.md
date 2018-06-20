---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: L’élément AggregationRestriction spécifie une valeur qui est appliquée à un ensemble de propriétés personnage résultant d’une demande FindPeople et filtre les résultats en fonction de la restriction spécifiée.
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755193"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

L’élément **AggregationRestriction** spécifie une valeur qui est appliquée à un ensemble de propriétés personnage résultant d’une demande FindPeople et filtre les résultats en fonction de la restriction spécifiée. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Remarques

L’élément **AggregationRestriction** peut contenir n’importe quel élément enfant qui utilise le groupe de substitution **SearchExpression** . Les éléments qui font partie du groupe de substitution **SearchExpression** sont : [Contains](contains.md), [exclut](excludes.md), [Exists](exists.md), [pas](not.md), [ou](or.md) [et](and.md), [plutôt IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan ](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)et [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

