---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: L’élément ContextFolderId indique le dossier ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible.
ms.openlocfilehash: 60f1eaf3b45eee83632c7da6f453a1d09f54d9fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529258"
---
# <a name="contextfolderid"></a>ContextFolderId

L’élément **ContextFolderId** indique le dossier ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible. 
  
- [ApplyConversationAction](applyconversationaction.md) 
- [ConversationActions](conversationactions.md)
- [ConversationAction](conversationaction.md)
- [ContextFolderId](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification du dossier de contexte.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers qui peuvent être référencés par leur nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une conversation unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)

