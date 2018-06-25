---
title: TaskSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ade9ea3b-bdf1-4999-ac7d-44c6452cef36
description: L’élément TaskSuggestion contient une suggestion de tâche qui résulte d’une entité extraite d’un élément.
ms.openlocfilehash: bf12c3dc8b58b6be873e0a9b0863c80051eb4e11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838675"
---
# <a name="tasksuggestion"></a>TaskSuggestion

L’élément **TaskSuggestion** contient une suggestion de tâche qui résulte d’une entité extraite d’un élément. 
  
```XML
<TaskSuggestion>
   <Position/>
   <TaskString/>
   <Assignees/>
</TaskSuggestion>
```

**TaskSuggestionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Position](position.md) | [TaskString](taskstring.md) | [intervenants](assignees.md)
  
### <a name="parent-elements"></a>Éléments parents

[TaskSuggestions](tasksuggestions.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

