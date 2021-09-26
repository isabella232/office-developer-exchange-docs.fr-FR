---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: L’élément AddressListId spécifie l’identificateur d’une liste d’adresses.
ms.openlocfilehash: 5348c6877e24fcc0c8873df1098f8a8e30fe4c1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541559"
---
# <a name="addresslistid"></a>AddressListId

**L’élément AddressListId** spécifie l’identificateur d’une liste d’adresses. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Identificateur de liste d’adresses de chaîne. Cet attribut est obligatoire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, de la suppression, du déplacement et de la définition de l’état de lecture sur les éléments de conversation dans un dossier cible.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Spécifie l’identificateur du dossier dans lequel les éléments de courrier électronique sont copiés.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination pour les actions de copie et de déplacement.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Spécifie l’identificateur du dossier vers lequel les éléments de courrier électronique sont déplacés  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

