---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: L’élément SortBy contient une propriété Item utilisée pour trier le résultat de la recherche.
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468396"
---
# <a name="sortby"></a>SortBy

L’élément **SortBy** contient une propriété Item utilisée pour trier le résultat de la recherche. 
  
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
|Commande  <br/> |La valeur de texte de l’attribut **Order** est l’ordre de tri. Une valeur de texte **croissant** indique que les résultats sont triés par ordre croissant. Une valeur de texte **décroissant** indique que les résultats sont triés par ordre décroissant.  <br/> |
   
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
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

