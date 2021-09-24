---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: L’élément MoveItem définit une demande de déplacement d’un élément dans la Exchange store.
ms.openlocfilehash: 5df569722534b8a248da64b71f21219866173aab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509601"
---
# <a name="moveitem"></a>MoveItem

**L’élément MoveItem** définit une demande de déplacement d’un élément dans Exchange store. 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 **MoveItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |Représente le dossier de destination d’un élément déplacé.  <br/> |
|[ItemIds](itemids.md) <br/> |Contient un tableau d’éléments identifiés à déplacer vers le dossier représenté par [l’élément ToFolderId.](tofolderid.md)  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |Indique si les identificateurs d’élément des nouveaux éléments sont renvoyés dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

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



[Opération MoveItem](moveitem-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

