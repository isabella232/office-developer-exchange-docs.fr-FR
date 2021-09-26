---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: L’élément DestinationFolderId indique le dossier de destination pour les actions de copie et de déplacement.
ms.openlocfilehash: abdb91dd8b9b005d0721f4dcf38766c280effe97
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542385"
---
# <a name="destinationfolderid"></a>DestinationFolderId

**L’élément DestinationFolderId** indique le dossier de destination pour les actions de copie et de déplacement. 
  
- [ApplyConversationAction](applyconversationaction.md)  
- [ConversationActions](conversationactions.md) 
- [ConversationAction](conversationaction.md)  
- [DestinationFolderId](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

```XML
<DestinationFolderId>
   <DistinguishedFolderId/>
</DestinationFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification du dossier de destination.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers qui peuvent être référencés par leur nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une seule conversation.  <br/> |
   
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

