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
description: L’élément Data contient les données d’un seul élément exporté ou d’un élément à charger dans une boîte aux lettres.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526969"
---
# <a name="data-base64binary"></a>Données (base64Binary)

L’élément **Data** contient les données d’un seul élément exporté ou d’un élément à charger dans une boîte aux lettres. 
  
```XML
<Data/>
```

**XS : base64Binary**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande d’exportation d’un seul élément de boîte aux lettres.  <br/> |
|[Élément (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un élément unique à télécharger dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

L’élément **Data** contient les valeurs et les noms des propriétés d’un élément exporté ou d’un élément qui sera chargé dans une boîte aux lettres. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma de message  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md)
- [Opération UploadItems](uploaditems-operation.md)

