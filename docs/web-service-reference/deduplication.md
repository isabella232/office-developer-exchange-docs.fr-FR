---
title: Déduplication
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: L’élément Deduplication indique si le résultat de la recherche doit supprimer les éléments en double.
ms.openlocfilehash: 6178502d102b8c24b39d7276352c31740c62352c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543407"
---
# <a name="deduplication"></a>Déduplication

**L’élément Deduplication** indique si le résultat de la recherche doit supprimer les éléments en double. 
  
```XML
<Deduplication> true | false </Deduplication>
```

**Boolean**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** l’élément Deduplication indique que les résultats de la recherche peuvent ne pas contenir d’éléments en double. La valeur **false indique que** les résultats de la recherche peuvent contenir des éléments en double. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

