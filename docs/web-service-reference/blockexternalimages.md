---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: L’élément BlockExternalImages spécifie si les images externes sont bloquées dans les corps de texte HTML.
ms.openlocfilehash: 82ddb7e53f351324783fa39e3b76c9c0534b8193
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543582"
---
# <a name="blockexternalimages"></a>BlockExternalImages

**L’élément BlockExternalImages spécifie** si les images externes sont bloquées dans les corps de texte HTML. 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés de dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.  <br/> |
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés et le contenu de l’élément à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** **l’élément BlockExternalImages** indique que les images externes sont bloquées dans les corps HTML. La valeur **false indique** que les images externes sont autorisées. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

