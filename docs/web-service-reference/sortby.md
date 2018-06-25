---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: L’élément SortBy contient une propriété d’élément utilisée pour trier le résultat de recherche.
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829518"
---
# <a name="sortby"></a>SortBy

L’élément **SortBy** contient une propriété d’élément utilisée pour trier le résultat de recherche. 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Order  <br/> |La valeur de texte de l’attribut **ordre** est l’ordre de tri. Une valeur texte **croissant** indique que les résultats sont dans l’ordre croissant. Une valeur texte **décroissant** indique que les résultats sont dans l’ordre décroissant.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchMailboxes](searchmailboxes.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

