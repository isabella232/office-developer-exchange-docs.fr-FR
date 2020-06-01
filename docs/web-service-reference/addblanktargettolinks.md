---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: L’élément AddBlankTargetToLinks spécifie que l’attribut cible des liens HTML est configuré pour ouvrir une nouvelle fenêtre.
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465042"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

L’élément **AddBlankTargetToLinks** spécifie que l’attribut cible des liens HTML est configuré pour ouvrir une nouvelle fenêtre. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**XS : Boolean**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés d’élément et le contenu à inclure dans une réponse **GetItem**, **FindItem**, **GetConversationItems** ou **SyncFolderItems** .<br/><br/>  Voici les expressions XPath de cet élément :<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **AddBlankTargetToLinks** indique que tous les liens html seront définis pour ouvrir une nouvelle fenêtre. La valeur **false** indique que les liens html s’ouvrent dans la fenêtre active. 
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

