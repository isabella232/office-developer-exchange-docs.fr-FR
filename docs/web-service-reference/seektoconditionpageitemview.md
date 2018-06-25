---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: L’élément SeekToConditionPageItemView identifie la condition est utilisée pour identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour une recherche FindItem ou FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829328"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

L’élément **SeekToConditionPageItemView** identifie la condition est utilisée pour identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour un **FindItem** ou un **FindConversation **recherche. 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Point de base  <br/> |La valeur de texte de l’attribut de **point de base** est le point de base à partir de dans laquelle la recherche est lancée. Une valeur de texte de **début** indique que la recherche commence au début du jeu de résultats. Une valeur de texte **fin** indique que la recherche démarre à la fin du jeu de résultats.  <br/> |
|MaxEntriesReturned  <br/> |La valeur de texte de l’attribut **MaxEntriesReturned** est le nombre maximal d’éléments pouvant être renvoyés dans un jeu de résultats.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[Condition (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindConversation](findconversation.md) | [FindItem](finditem.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

