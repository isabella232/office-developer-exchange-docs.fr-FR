---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: L’élément MaxItems spécifie le nombre maximal d’éléments à renvoyer dans la demande.
ms.openlocfilehash: f16e9d46b59c0f562aabd5383f7f445d93414f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461743"
---
# <a name="maxitems"></a>MaxItems

L’élément **MaxItems** spécifie le nombre maximal d’éléments à renvoyer dans la demande. 
  
```XML
<MaxItems/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **MaxItems** est le nombre maximal d’éléments à renvoyer dans la demande. Ce nombre ne peut pas être inférieur à zéro ou supérieur à 200. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[GetReminders](getreminders.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

