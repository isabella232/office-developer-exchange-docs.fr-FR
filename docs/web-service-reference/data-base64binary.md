---
title: Data (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: L’élément Data contient les données d’un élément exporté unique ou d’un élément à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 69e15746f17febb74a0ec2f56eef0eaa1e298015
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535933"
---
# <a name="data-base64binary"></a>Data (base64Binary)

**L’élément Data** contient les données d’un élément exporté unique ou d’un élément à télécharger dans une boîte aux lettres. 
  
```XML
<Data/>
```

**xs:base64Binary**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande d’exportation d’un élément de boîte aux lettres unique.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un élément unique à télécharger dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

**L’élément Data** contient les noms et valeurs des propriétés d’un élément exporté ou d’un élément qui sera chargé dans une boîte aux lettres. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md)
- [Opération UploadItems](uploaditems-operation.md)

