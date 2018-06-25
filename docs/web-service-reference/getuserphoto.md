---
title: GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0e524a09-86f8-4a71-ac5c-66527ae70790
description: L’élément GetUserPhoto contient la requête pour obtenir la photo d’un utilisateur.
ms.openlocfilehash: 1fa1db6d903f83ad54ffadb188ba79ee178de797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827695"
---
# <a name="getuserphoto"></a>GetUserPhoto

L’élément **GetUserPhoto** contient la requête pour obtenir la photo d’un utilisateur. 
  
```XML
<GetUserPhoto>
   <Email/>
   <SizeRequested/>
</GetUserPhoto>
```

 **GetUserPhotoType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Courrier électronique (String)](email-string.md) | [SizeRequested](sizerequested.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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
   

