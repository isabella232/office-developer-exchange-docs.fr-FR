---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: L’élément MovedItemId spécifie l’identificateur de l’élément déplacé par l’opération MarkAsJunk.
ms.openlocfilehash: 0775aaed119242fc2a2057fb20807d5be30692e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509594"
---
# <a name="moveditemid"></a>MovedItemId

**L’élément MovedItemId** spécifie l’identificateur de l’élément déplacé par l’opération **MarkAsJunk.** 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de **l’attribut Id** est l’identificateur d’élément de l’élément déplacé par l’opération **MarkAsJunk.** L’identificateur d’élément reste le même après le déplacement.  <br/> |
|ChangeKey  <br/> |La valeur de **l’attribut ChangeKey** est la clé de modification de l’élément déplacé. La touche de modification change une fois que l’élément a été déplacé par **l’opération MarkAsJunk.**  <br/> |
   
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

