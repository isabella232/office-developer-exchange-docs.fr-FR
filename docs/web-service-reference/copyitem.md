---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: L’élément CopyItem définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755668"
---
# <a name="copyitem"></a>CopyItem

L’élément **CopyItem** définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange. 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 **CopyItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |Représente le dossier de destination pour un élément copié.  <br/> |
|[ItemId](itemids.md) <br/> |Contient un tableau d’éléments identifiés à copier dans le dossier représenté par l’élément [ToFolderId](tofolderid.md) .  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |Indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CopyItem](copyitem-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

