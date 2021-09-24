---
title: Updates (Item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: L’élément Updates contient un ensemble d’éléments qui définissent l’application, la définition et la suppression des modifications apportées aux propriétés d’élément.
ms.openlocfilehash: b4a343d941d29e9b25ebedfbf25894c7ec9b22d7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517405"
---
# <a name="updates-item"></a>Updates (Item)

**L’élément Updates** contient un ensemble d’éléments qui définissent l’application, la définition et la suppression des modifications apportées aux propriétés d’élément. 
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Mises à jour (élément)](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

**NonEmptyArrayOfItemChangeDescriptionsType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AppendToItemField](appendtoitemfield.md) <br/> |Représente les données à append à une propriété unique d’un élément lors d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Représente une opération de suppression d’une propriété donnée d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.  <br/> Voici l’expression XPath de cet élément :  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Les mises à jour définies par cet élément sont effectuées sur l’élément identifié par les éléments [ItemId,](itemid.md) [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId.](recurringmasteritemid.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |schéma types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération UpdateItem](updateitem-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

