---
title: HasChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 15ff513d-f39e-44ed-a13f-ab3f86fa37e1
description: L’élément HasChanged indique si la photo d’un utilisateur a changé.
ms.openlocfilehash: 456660272815aac27ea99919eb92a02f754fb4ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516789"
---
# <a name="haschanged"></a>HasChanged

**L’élément HasChanged** indique si la photo d’un utilisateur a changé. 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetUserPhotoResponse](getuserphotoresponse.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** l’élément **HasChanged** indique que la photo a changé depuis la dernière fois qu’elle a été renvoyée. La valeur **false indique** que la photo n’a pas changé depuis la dernière fois qu’elle a été renvoyée. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

