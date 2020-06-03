---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: L’élément SizeRequested contient la taille de photo demandée pour une opération GetUserPhoto.
ms.openlocfilehash: 2e79bbb158fa9a22cbd3ec08fcd6e60429e113b4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460455"
---
# <a name="sizerequested"></a>SizeRequested

L’élément **SizeRequested** contient la taille de photo demandée pour une opération **GetUserPhoto** . 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **SizeRequested** est la taille de photo demandée d’une image numérique renvoyée à partir du serveur. Le tableau suivant identifie les valeurs de texte de l’élément **SizeRequested** . 
  
|**Valeur**|**Signification**|
|:-----|:-----|
|HR48x48  <br/> |La hauteur de l’image est de 48 pixels et de 48 pixels.  <br/> |
|HR64x64  <br/> |La hauteur de l’image est de 64 pixels et de 64 pixels.  <br/> |
|HR96x96  <br/> |La hauteur de l’image est de 96 pixels et de 96 pixels.  <br/> |
|HR120x120  <br/> |La hauteur de l’image est de 120 pixels et de 120 pixels.  <br/> |
|HR240x240  <br/> |La hauteur de l’image est de 240 pixels et de 240 pixels.  <br/> |
|HR360x360  <br/> |La hauteur de l’image est de 360 pixels et de 360 pixels.  <br/> |
|HR432x432  <br/> |La hauteur de l’image est de 432 pixels et de 432 pixels.  <br/> |
|HR504x504  <br/> |La hauteur de l’image est de 504 pixels et de 504 pixels.  <br/> |
|HR648x648  <br/> |La hauteur de l’image est de 648 pixels et de 648 pixels.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

