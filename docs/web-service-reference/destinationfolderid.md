---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: L’élément DestinationFolderId indique le dossier de destination de copie et les actions de déplacement.
ms.openlocfilehash: 5fb6cae7db9cdb09e23b3627e26e695ecf6418f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755906"
---
# <a name="destinationfolderid"></a>DestinationFolderId

L’élément **DestinationFolderId** indique le dossier de destination de copie et les actions de déplacement. 
  
- [ApplyConversationAction](applyconversationaction.md)  
- [ConversationActions](conversationactions.md) 
- [ConversationAction](conversationaction.md)  
- [DestinationFolderId](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et modification du dossier de destination.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers qui peuvent être référencés par un nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une même conversation.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)

