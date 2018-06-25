---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: L’élément BlockExternalImages Spécifie si les images externes sont bloqués dans le corps de texte HTML.
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755388"
---
# <a name="blockexternalimages"></a>BlockExternalImages

L’élément **BlockExternalImages** Spécifie si les images externes sont bloqués dans le corps de texte HTML. 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés du dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.  <br/> |
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **BlockExternalImages** indique que des images externes sont bloqués dans le corps HTML. La valeur **false** indique que les images externes sont autorisées. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

