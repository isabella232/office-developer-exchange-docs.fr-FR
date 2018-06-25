---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: L’élément AddressListId Spécifie l’identificateur d’une liste d’adresses.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755185"
---
# <a name="addresslistid"></a>AddressListId

L’élément **AddressListId** Spécifie l’identificateur d’une liste d’adresses. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Identificateur de liste adresse chaîne. Cet attribut est requis.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, suppression, déplacement et en définissant l’état de lecture sur les éléments de conversation dans un dossier cible.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Spécifie l’identificateur du dossier dans lequel sont copiés les éléments de messagerie électronique.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination de copie et les actions de déplacement.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Spécifie l’identificateur du dossier vers lequel les éléments de messagerie électronique sont déplacés  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

