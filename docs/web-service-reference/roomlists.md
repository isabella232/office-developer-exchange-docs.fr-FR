---
title: RoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: L’élément RoomLists est une liste d’une ou plusieurs adresses qui représentent une liste de salles de réunion.
ms.openlocfilehash: e2825ccf5f660e00da61a605282613c07678a74b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523488"
---
# <a name="roomlists"></a>RoomLists

**L’élément RoomLists** est une liste d’une ou plusieurs adresses qui représentent une liste de salles de réunion. 
  
[GetRoomListsResponse](getroomlistsresponse.md)
  
[RoomLists](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 **ArrayOfEmailAddressesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Adresse (EmailAddressType)](address-emailaddresstype.md) <br/> |Définit l’adresse de messagerie et le nom complet qui représente la liste des salles. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetRoomLists.](getroomlists-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetRoomLists](getroomlists-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

