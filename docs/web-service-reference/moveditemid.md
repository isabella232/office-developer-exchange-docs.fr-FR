---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: L’élément MovedItemId spécifie l’identificateur de l’élément qui a été déplacé par l’opération MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468613"
---
# <a name="moveditemid"></a>MovedItemId

L’élément **MovedItemId** spécifie l’identificateur de l’élément qui a été déplacé par l’opération **MarkAsJunk** . 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de l’attribut **ID** est l’identificateur d’élément de l’élément qui est déplacé par l’opération **MarkAsJunk** . L’identificateur de l’élément reste le même après le déplacement.  <br/> |
|ChangeKey  <br/> |La valeur de l’attribut **ChangeKey** est la clé de modification de l’élément déplacé. La modification de la clé change après le déplacement de l’élément par l’opération **MarkAsJunk** .  <br/> |
   
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
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

