---
title: Mises à jour (élément)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: L’élément de mises à jour contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément.
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838914"
---
# <a name="updates-item"></a>Mises à jour (élément)

L’élément de **mises à jour** contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AppendToItemField](appendtoitemfield.md) <br/> |Représente les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Représente une opération de suppression d’une propriété donnée d’un élément pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>Remarques

Les mises à jour qui sont définies par cet élément sont effectuées sur l’élément identifié par les éléments [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |schéma de types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [UpdateItem Operation](updateitem-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

