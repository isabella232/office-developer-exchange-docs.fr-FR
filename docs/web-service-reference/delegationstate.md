---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: L’élément DelegationState représente l’état d’une tâche déléguée.
ms.openlocfilehash: 218e96b73c1681bd9bb2fd964a735b62b9e2a94b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542504"
---
# <a name="delegationstate"></a>DelegationState

**L’élément DelegationState** représente l’état d’une tâche déléguée. 
  
```xml
<DelegationState/>
```

**TaskDelegateStateType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Il s’agit d’une propriété en lecture seule. Les valeurs possibles sont les suivantes :
  
- NoMatch
    
- OwnNew
    
- Owned
    
- Accepted
    
- Refusée
    
- Max
    
## <a name="remarks"></a>Remarques

Exchange Les services web Microsoft Exchange Server 2007 ne prend pas en charge les affectations de tâches.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange 2007 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

