---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: L’élément ItemChange contient un identificateur d’élément et les mises à jour à appliquer à l’élément.
ms.openlocfilehash: 8ace3cf78eb902e48529a0534e39ce7d584bd164
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537748"
---
# <a name="itemchange"></a>ItemChange

**L’élément ItemChange** contient un identificateur d’élément et les mises à jour à appliquer à l’élément. 
  
- [UpdateItem](updateitem.md) 
- [ItemChanges](itemchanges.md)
- [ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

**ItemChangeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange. Cet élément est requis si [l’élément OccurrenceItemId](occurrenceitemid.md) ou [RecurringMasterItemId](recurringmasteritemid.md) n’est pas utilisé.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifie une occurrence unique d’un élément périodique. Cet élément est requis s’il est utilisé. Cet élément est requis si [l’élément RecurringMasterItemId](recurringmasteritemid.md) ou [ItemId](itemid.md) n’est pas utilisé.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifie un élément récurrence maître en identifiant l’un de ses identificateurs d’éléments d’occurrence associés. Cet élément est requis s’il est utilisé. Cet élément est requis si [l’élément OccurrenceItemId](occurrenceitemid.md) ou [ItemId](itemid.md) n’est pas utilisé.  <br/> |
|[Mises à jour (élément)](updates-item.md) <br/> |Contient un tableau qui définit l’application, la définition et la suppression des modifications apportées aux propriétés d’élément. Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |Contient un tableau [d’éléments ItemChange](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Remarques

Un seul [élément ItemId,](itemid.md) [OccurrenceItemId](occurrenceitemid.md)ou [RecurringMasterItemId](recurringmasteritemid.md) peut être utilisé dans un **élément ItemChange.** 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [UpdateItem Operation](updateitem-operation.md)

