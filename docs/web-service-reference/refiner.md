---
title: Affinement
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8395b45f-3b94-4473-82ac-2a12c4309170
description: L’élément de perfectionnement spécifie un affinement de recherche.
ms.openlocfilehash: aad1874760e02b2226cbe1a5bb700013d3816cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829038"
---
# <a name="refiner"></a>Affinement

L’élément de **perfectionnement** spécifie un affinement de recherche. 
  
```XML
<Refiner>
   <Name/>
   <Value/>
   <Count/>
   <Token/>
</Refiner>
```

 **SearchRefinerItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Name (chaîne)](name-string.md) | [valeur](value.md) | [Count](count.md) | [jeton (chaîne)](token-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[Affinements](refiners.md)
  
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
   

