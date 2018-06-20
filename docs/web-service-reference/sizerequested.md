---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: L’élément SizeRequested contient la taille de photo demandé pour une opération GetUserPhoto.
ms.openlocfilehash: 43e422512b1e8f06e410e533e9ae1dc49283d5f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829504"
---
# <a name="sizerequested"></a>SizeRequested

L’élément **SizeRequested** contient la taille de photo demandé pour une opération **GetUserPhoto** . 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **SizeRequested** est la taille de photo demandé d’une image numérique renvoyée à partir du serveur. Le tableau suivant identifie les valeurs de texte de l’élément **SizeRequested** . 
  
|**Valeur**|**Signification**|
|:-----|:-----|
|HR48x48  <br/> |L’image est 48 pixels et 48 pixels de large.  <br/> |
|HR64x64  <br/> |L’image est de 64 pixels et 64 pixels de large.  <br/> |
|HR96x96  <br/> |L’image est 96 pixels et 96 pixels de large.  <br/> |
|HR120x120  <br/> |L’image est 120 pixels de haut et 120 pixels de large.  <br/> |
|HR240x240  <br/> |L’image est de 240 pixels et 240 pixels de large.  <br/> |
|HR360x360  <br/> |L’image est 360 pixels de haut et 360 pixels de large.  <br/> |
|HR432x432  <br/> |L’image est 432 pixels de haut et 432 pixels de large.  <br/> |
|HR504x504  <br/> |L’image est 504 pixels de haut et 504 pixels de large.  <br/> |
|HR648x648  <br/> |L’image est 648 pixels de haut et 648 pixels de large.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

