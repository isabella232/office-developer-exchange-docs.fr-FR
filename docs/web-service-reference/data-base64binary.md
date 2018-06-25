---
title: Données (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: L’élément de données contient les données d’un seul élément exporté ou un élément à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755786"
---
# <a name="data-base64binary"></a>Données (base64Binary)

L’élément de **données** contient les données d’un seul élément exporté ou un élément à télécharger dans une boîte aux lettres. 
  
```XML
<Data/>
```

**xs : base64Binary**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande pour exporter un élément de boîte aux lettres unique.  <br/> |
|[Élément (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un seul élément à télécharger dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

L’élément de **données** contient les noms de propriétés et les valeurs d’un élément exporté ou un élément dans une boîte aux lettres sera téléchargé. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md)
- [Opération UploadItems](uploaditems-operation.md)

