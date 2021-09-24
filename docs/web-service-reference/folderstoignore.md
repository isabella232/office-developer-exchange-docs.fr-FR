---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: L’élément FoldersToIgnore identifie une liste de dossiers qui sont ignorés lors de l’obtention d’éléments dans une conversation. Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse GetConversationItems.
ms.openlocfilehash: c0102d12b24df2cadd5e307e80c5acda9a3c0589
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528659"
---
# <a name="folderstoignore"></a>FoldersToIgnore

**L’élément FoldersToIgnore** identifie une liste de dossiers qui sont ignorés lors de l’obtention d’éléments dans une conversation. Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse **GetConversationItems.** 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[FolderId](folderid.md)  |  [DistinguishedFolderId](distinguishedfolderid.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetConversationItems](getconversationitems.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

