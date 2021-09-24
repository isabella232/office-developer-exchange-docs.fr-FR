---
title: SearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: eb0a7897-c642-4c93-a238-be03128af54e
description: L’élément SearchableMailboxes contient un tableau des boîtes aux lettres renvoyées par une demande GetSearchableMailboxes.
ms.openlocfilehash: 5d8b1f19a4d4e2e78ab4d4a251d3c7538ccdd9ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510840"
---
# <a name="searchablemailboxes"></a>SearchableMailboxes

**L’élément SearchableMailboxes contient** un tableau des boîtes aux lettres renvoyées par une **demande GetSearchableMailboxes.** 
  
```XML
<SearchableMailboxes>
   <SearchableMailbox/>
</SearchableMailboxes>
```

 **ArrayOfSearchableMailboxesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[SearchableMailbox](searchablemailbox.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

