---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: L’élément MaximumSize représente la taille maximale doit correspondre à un message afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 37e3d377b105534fe34b54e262bd47bc450706da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828387"
---
# <a name="maximumsize"></a>MaximumSize

L’élément **MaximumSize** représente la taille maximale doit correspondre à un message afin que l’exception ou la condition à appliquer. 
  
```XML
<Maximum/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie les tailles minimales et maximales des messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est un entier qui identifie la taille maximale du message en octets.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[MinimumSize](minimumsize.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

