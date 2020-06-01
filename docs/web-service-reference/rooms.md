---
title: Salons
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rooms
api_type:
- schema
ms.assetid: 57b6079a-3d83-4429-861e-c551e9e1a991
description: L’élément Rooms est une liste d’un ou plusieurs éléments qui représentent des salles de réunion.
ms.openlocfilehash: f8b60a9680f6abba459ebecc96613abfdd93766d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466184"
---
# <a name="rooms"></a>Salons

L’élément **rooms** est une liste d’un ou plusieurs éléments qui représentent des salles de réunion. 
  
[GetRoomsResponse](getroomsresponse.md)
  
[Salons](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 **ArrayOfRoomsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Salle](room.md) <br/> |Définit une adresse de messagerie et un nom d’affichage qui représente une salle de réunion.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetRoomsResponse](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetRooms](getrooms-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

