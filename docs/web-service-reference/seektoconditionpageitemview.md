---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: L’élément SeekToConditionPageItemView identifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et les instructions de recherche pour une recherche FindItem ou FindConversation.
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466835"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

L’élément **SeekToConditionPageItemView** identifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation** . 
  
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
|BasePoint  <br/> |La valeur de texte de l’attribut **BasePoint** est le point de base de l’emplacement de démarrage de la recherche. Une valeur de **départ** indique que la recherche commence au début du jeu de résultats. Une valeur de **fin** indique que la recherche commence à la fin du jeu de résultats.  <br/> |
|MaxEntriesReturned  <br/> |La valeur de texte de l’attribut **MaxEntriesReturned** est le nombre maximal d’éléments qui peuvent être renvoyés dans un jeu de résultats.  <br/> |
   
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
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

