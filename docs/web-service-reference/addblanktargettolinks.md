---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: L’élément AddBlankTargetToLinks spécifie que l’attribut cible dans les liaisons HTML est définie pour ouvrir une nouvelle fenêtre.
ms.openlocfilehash: c8d7a5973e60e43638472b0da29842ce1caacc98
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543827"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

**L’élément AddBlankTargetToLinks** spécifie que l’attribut cible dans les liaisons HTML est définie pour ouvrir une nouvelle fenêtre. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs:Boolean**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une réponse **GetItem,** **FindItem,** **GetConversationItems** ou **SyncFolderItems.**<br/><br/>  Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **AddBlankTargetToLinks** indique que tous les liens HTML seront définies pour ouvrir une nouvelle fenêtre. La valeur **false indique** que les liens HTML s’ouvrent dans la fenêtre actuelle. 
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
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

