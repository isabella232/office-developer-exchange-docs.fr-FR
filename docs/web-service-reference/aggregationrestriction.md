---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: L’élément AggregationRestriction spécifie une valeur qui est appliquée à un ensemble de propriétés Persona résultant d’une demande FindPeople et filtre le résultat en fonction de la restriction spécifiée.
ms.openlocfilehash: 6a00035f87e0f365f4551df1a6ff570e01761770
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546790"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

**L’élément AggregationRestriction** spécifie une valeur qui est appliquée à un ensemble de propriétés Persona résultant d’une demande FindPeople et filtre le résultat en fonction de la restriction spécifiée. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Remarques

**L’élément AggregationRestriction** peut contenir n’importe quel élément enfant qui utilise le groupe de substitution **SearchExpression.** Les éléments qui font partie du groupe de substitution **SearchExpression** sont : [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md) [,](or.md)Or , [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)et [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

