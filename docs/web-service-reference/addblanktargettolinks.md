---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: L’élément AddBlankTargetToLinks indique que l’attribut cible des liens HTML sont définies pour ouvrir une nouvelle fenêtre.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755158"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

L’élément **AddBlankTargetToLinks** indique que l’attribut cible des liens HTML sont définies pour ouvrir une nouvelle fenêtre. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs : Boolean**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés de l’élément et le contenu à inclure dans une **GetItem**, **FindItem**, **GetConversationItems** ou une réponse **SyncFolderItems** .<br/><br/>  Les expressions XPath pour cet élément sont les suivantes :<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **AddBlankTargetToLinks** indique que tous les liens HTML seront définies pour ouvrir une nouvelle fenêtre. La valeur **false** indique que les liens HTML seront ouvre dans la fenêtre active. 
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
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

