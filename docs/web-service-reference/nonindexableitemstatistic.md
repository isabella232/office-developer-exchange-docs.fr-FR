---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: L’élément NonIndexableItemStatistic contient une statistique unique pour un élément qui ne peut pas être indexé.
ms.openlocfilehash: e604f73216aab4cca259bc6cb7eb80a2fd36cd23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828540"
---
# <a name="nonindexableitemstatistic"></a>NonIndexableItemStatistic

L’élément **NonIndexableItemStatistic** contient une statistique unique pour un élément qui ne peut pas être indexé. 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 **NonIndexableItemStatisticType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Boîte aux lettres (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)
  
### <a name="parent-elements"></a>Éléments parents

[NonIndexableItemStatistics](nonindexableitemstatistics.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

