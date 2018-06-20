---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: L’élément ItemChange contient un identificateur d’élément et les mises à jour à appliquer à l’élément.
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828145"
---
# <a name="itemchange"></a>ItemChange

L’élément **ItemChange** contient un identificateur d’élément et les mises à jour à appliquer à l’élément. 
  
[UpdateItem](updateitem.md)
  
[ItemChanges](itemchanges.md)
  
[ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

 **ItemChangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID d’élément](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange. Cet élément est obligatoire si l’élément [OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) n’est pas utilisée.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifie une seule occurrence d’un élément périodique. Cet élément est requis en cas d’utilisation. Cet élément est obligatoire si l’élément [RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) n’est pas utilisée.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifie un élément de gabarit périodicité en identifiant un des identificateurs des éléments de son occurrence connexes. Cet élément est requis en cas d’utilisation. Cet élément est obligatoire si l’élément [OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) n’est pas utilisée.  <br/> |
|[Mises à jour (élément)](updates-item.md) <br/> |Contient un tableau qui définit append, définir et supprimer les modifications apportées aux propriétés de l’élément. Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |Contient un tableau d’éléments [ItemChange](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Remarques

Qu’un seul élément [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) peut être utilisé dans un élément **ItemChange** . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)

