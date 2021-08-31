---
title: Modifications (éléments)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: L’élément Changes contient un tableau de séquences de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur Exchange serveur.
ms.openlocfilehash: ede81d8ecae9751c477ae05cbd13f914fedf8e0f
ms.sourcegitcommit: 357b882a02e37b380a23b8a45b15f9c006a40b02
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58764629"
---
# <a name="changes-items"></a>Modifications (éléments)

**L’élément Changes** contient un tableau de séquences de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur Exchange serveur. 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[Modifications (éléments)](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
   <ReadFlagChange/>
</Changes>
```

 **SyncFolderItemsChangesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Créer (ItemSync)](create-itemsync.md) <br/> |Identifie un élément unique à créer dans le magasin de clients local.  <br/> |
|[Mise à jour (ItemSync)](update-itemsync.md) <br/> |Identifie un élément unique à mettre à jour dans le magasin de client local.  <br/> |
|[Delete (ItemSync)](delete-itemsync.md) <br/> |Identifie un élément unique à supprimer dans le magasin de clients local.  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |Renvoyé dans [les réponses de l’opération SyncFolderItems](syncfolderitems-operation.md) lorsqu’un élément a été lu. Cette propriété est en lecture seule.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération SyncFolderItems.](syncfolderitems-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

