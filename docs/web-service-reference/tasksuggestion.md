---
title: TaskSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ade9ea3b-bdf1-4999-ac7d-44c6452cef36
description: L’élément TaskSuggestion contient une suggestion de tâche résultant d’une entité extraite d’un élément.
ms.openlocfilehash: a7d74523b57825b97c6c6d9c2194d84af3f38d5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538876"
---
# <a name="tasksuggestion"></a>TaskSuggestion

**L’élément TaskSuggestion** contient une suggestion de tâche résultant d’une entité extraite d’un élément. 
  
```XML
<TaskSuggestion>
   <Position/>
   <TaskString/>
   <Assignees/>
</TaskSuggestion>
```

**TaskSuggestionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Position](position.md)  |  [TaskString](taskstring.md)  |  [Personnes assignées](assignees.md)
  
### <a name="parent-elements"></a>Éléments parents

[TaskSuggestions](tasksuggestions.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

