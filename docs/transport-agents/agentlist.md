---
title: agentList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: eadae2a22e4c844f1f2edce9211100bb9ef2776d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529355"
---
# <a name="agentlist"></a>agentList
  
**S’applique à :** Exchange Server 2013
  
**L’élément agentList** contient un [élément agent](agent.md) pour chaque agent installé. 
  
- [configuration](configuration.md)
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

**agentListType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[agent](agent.md) <br/> |Contient des informations de configuration sur un agent installé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration pour la surveillance des agents et les informations de configuration sur les agents installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

