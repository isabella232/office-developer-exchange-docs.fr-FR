---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: L’élément SortBy contient une propriété d’élément utilisée pour trier les résultats de la recherche.
ms.openlocfilehash: 8718bad3749a0409be2715b0e03001b97a4fb87e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544688"
---
# <a name="sortby"></a>SortBy

**L’élément SortBy** contient une propriété d’élément utilisée pour trier les résultats de la recherche. 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Commande  <br/> |La valeur de texte de **l’attribut Order** est l’ordre de tri. Une valeur de texte **Ascending** indique que les résultats sont dans l’ordre croissant. Une valeur de texte **Décroit** indique que les résultats sont dans l’ordre décroit.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[FieldURI](fielduri.md)  |  [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxes](searchmailboxes.md)
  
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
   

