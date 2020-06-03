---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: L’élément ReadFlag indique l’état de lecture à définir sur les éléments d’un dossier.
ms.openlocfilehash: 1d3b9f3fe199ed2e63bdb632135120a5f89f4d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529895"
---
# <a name="readflag"></a>ReadFlag

L’élément **ReadFlag** indique l’état de lecture à définir sur les éléments d’un dossier. 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MarkAllItemsAsRead](markallitemsasread.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **ReadFlag** indique que les éléments dans le dossier seront marqués comme lus. La valeur **false** indique que les éléments du dossier seront marqués comme non lus. 
  
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
   

