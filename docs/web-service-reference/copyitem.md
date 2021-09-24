---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: L’élément CopyItem définit une demande de copie d’un élément dans une boîte aux lettres dans Exchange store.
ms.openlocfilehash: 7f083f09a587b4788180711039e1cfdbbe6a10cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529175"
---
# <a name="copyitem"></a>CopyItem

**L’élément CopyItem** définit une demande de copie d’un élément dans une boîte aux lettres dans Exchange store. 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 **CopyItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |Représente le dossier de destination d’un élément copié.  <br/> |
|[ItemIds](itemids.md) <br/> |Contient un tableau d’éléments identifiés à copier dans le dossier représenté par [l’élément ToFolderId.](tofolderid.md)  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |Indique si les identificateurs d’élément des nouveaux éléments sont renvoyés dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CopyItem](copyitem-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

