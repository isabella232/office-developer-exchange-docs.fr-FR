---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: L’élément NonIndexableItemStatistic contient une statistique unique pour un élément qui n’a pas pu être indexé
ms.openlocfilehash: 93bdaad2f10adf52ef99f51106596f155af2f18c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509545"
---
# <a name="nonindexableitemstatistic"></a>NonIndexableItemStatistic

**L’élément NonIndexableItemStatistic** contient une statistique unique pour un élément qui n’a pas pu être indexé 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 **NonIndexableItemStatisticType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Boîte aux lettres (chaîne)](mailbox-string.md)  |  [ItemCount](itemcount.md)  |  [ErrorMessage](errormessage.md)
  
### <a name="parent-elements"></a>Éléments parents

[NonIndexableItemStatistics](nonindexableitemstatistics.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

