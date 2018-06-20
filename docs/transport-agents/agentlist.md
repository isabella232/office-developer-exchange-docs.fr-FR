---
title: agentList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755111"
---
# <a name="agentlist"></a>agentList
  
**S’applique à :** Exchange Server 2013
  
L’élément **agentList** contient un élément de [l’agent](agent.md) pour chaque agent installé. 
  
- [configuration](configuration.md)
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

**agentListType (type complexe)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[agent](agent.md) <br/> |Contient des informations de configuration sur un agent installé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Contient des éléments qui définissent les informations de configuration pour l’agent de surveillance et les informations de configuration sur les agents installés.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas un espace de noms.  <br/> |
|Nom du schéma  <br/> |N’est pas disponible.  <br/> |
|Fichier de validation  <br/> |N’est pas disponible.  <br/> |
|Peut être vide  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

