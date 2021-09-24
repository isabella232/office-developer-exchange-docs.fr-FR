---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: L’élément UpdateItemInRecoverableItems spécifie une demande de mise à jour d’un élément dans les éléments récupérables.
ms.openlocfilehash: 8d3ffdd2d3f60e48514ae1a9d7cb4ca4e1bf06ac
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515017"
---
# <a name="updateiteminrecoverableitems"></a>UpdateItemInRecoverableItems

**L’élément UpdateItemInRecoverableItems** spécifie une demande de mise à jour d’un élément dans les éléments récupérables. 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 **UpdateItemInRecoverableItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemid.md)  |  [Mises à jour (élément)](updates-item.md)  |  [Pièces jointes](attachments-ex15websvcsotherref.md)  |  [MakeItemImmutable](makeitemimmutable.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

