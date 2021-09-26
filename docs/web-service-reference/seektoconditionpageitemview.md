---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: L’élément SeekToConditionPageItemView identifie la condition utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, le nombre maximal d’entrées à renvoyer et les instructions de recherche pour une recherche FindItem ou FindConversation.
ms.openlocfilehash: 6f4797a6b90456a50922db1c829757711816273e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546104"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

L’élément **SeekToConditionPageItemView** identifie la condition utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, le nombre maximal d’entrées à renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation.** 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BasePoint  <br/> |La valeur de texte de **l’attribut BasePoint** est le point de base à partir de laquelle la recherche va commencer. Une valeur de texte **de Début** indique que la recherche commence au début du jeu de résultats. Une valeur de texte **End** indique que la recherche démarrera à la fin du jeu de résultats.  <br/> |
|MaxEntriesReturned  <br/> |La valeur de texte de **l’attribut MaxEntriesReturned** est le nombre maximal d’éléments qui peuvent être renvoyés dans un jeu de résultats.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[Condition (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindConversation](findconversation.md)  |  [FindItem](finditem.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

