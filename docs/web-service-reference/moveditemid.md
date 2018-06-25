---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: L’élément MovedItemId Spécifie l’identificateur de l’élément a été déplacé par l’opération MarkAsJunk.
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828484"
---
# <a name="moveditemid"></a>MovedItemId

L’élément **MovedItemId** Spécifie l’identificateur de l’élément a été déplacé par l’opération **MarkAsJunk** . 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de l’attribut **Id** est l’identificateur d’élément de l’élément est déplacé par l’opération **MarkAsJunk** . L’identificateur d’élément restent les mêmes après le déplacement.  <br/> |
|ChangeKey  <br/> |La valeur de l’attribut **ChangeKey** est la clé de modification de l’élément déplacé. Modifier la clé modifie une fois que l’élément est déplacé par l’opération **MarkAsJunk** .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

