---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: L’élément MakeItemImmutable spécifie une valeur de type Boolean qui indique si un élément doit être effectué en lecture seule.
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828337"
---
# <a name="makeitemimmutable"></a>MakeItemImmutable

L’élément **MakeItemImmutable** spécifie une valeur de type Boolean qui indique si un élément doit être effectué en lecture seule. 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[UpdateItemInRecoverableItems](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **MakeItemImmutable** indique que l’élément doit être mis en lecture seule. La valeur **false** indique que l’élément autorise l’accès en lecture-écriture. 
  
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
   

