---
title: Supprimer (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: L’élément Supprimer identifie un seul élément à supprimer dans le magasin de client local.
ms.openlocfilehash: 18b7ae2f97db2de64896680c3aa76f2590c03177
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755849"
---
# <a name="delete-itemsync"></a>Supprimer (ItemSync)

L’élément **Supprimer** identifie un seul élément à supprimer dans le magasin de client local. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Modifications (éléments)](changes-items.md)  
- [Supprimer (ItemSync)](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

**SyncFolderItemsDeleteType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID d’élément](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Modifications (éléments)](changes-items.md) <br/> |Contient un tableau de séquence de types de modification qui représente le type des différences entre les éléments sur le client et les éléments sur le serveur Exchange.  <br/> |
   
## <a name="remarks"></a>Note

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération SyncFolderItems](syncfolderitems-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

