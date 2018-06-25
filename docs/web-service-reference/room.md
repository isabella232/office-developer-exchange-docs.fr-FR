---
title: Salle
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Room
api_type:
- schema
ms.assetid: a2cde8b8-2d31-4ebf-8171-f4dfd650d079
description: L’élément salle représente une salle de réunion.
ms.openlocfilehash: e064a458b5a9265fc9dad63c87c641eaf47d7062
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829242"
---
# <a name="room"></a>Salle

L’élément **salle** représente une salle de réunion. 
  
[Salles](rooms.md)
  
[Salle](room.md)
  
```XML
<Room>
   <Id/>
</Room>
```

 **RoomType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID (EmailAddressType)](id-emailaddresstype.md) <br/> |Un identificateur qui contient une adresse de messagerie et le nom complet qui représente la salle de réunion.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Salles](rooms.md) <br/> |Définit une liste de salles associés à une fonctionnalité commune, comme étant situé dans le même bâtiment de réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetRooms](getrooms-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

