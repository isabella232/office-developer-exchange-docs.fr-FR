---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: L’élément OccurrenceItemId identifie une occurrence unique d’un élément périodique.
ms.openlocfilehash: ac6fc081e67f3897880ad30fcc1b62fe2e844459
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515417"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

**L’élément OccurrenceItemId** identifie une occurrence unique d’un élément périodique. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Identifie la maître périodique d’un élément périodique. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique du maître périodique ou une occurrence d’élément. Si la forme de maître périodique ou l’une de ses occurrences change, **changez ChangeKey.** **ChangeKey** est identique pour la maître périodique et toutes les occurrences.  <br/> |
|**InstanceIndex** <br/> |Identifie l’index de l’occurrence de l’élément. Cet attribut est obligatoire. Cette valeur représente un integer.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’éléments pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemIds](itemids.md) <br/> | Contient les identités uniques des éléments, des éléments d’occurrence et des éléments maîtres périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Exchange store. <br/><br/>Les expressions XPath de cet élément sont les suivantes : <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**REMARQUE**: [l’opération MoveItem et](moveitem-operation.md) [l’opération CopyItem](copyitem-operation.md) fonctionnent uniquement avec des éléments de calendrier et des éléments maîtres périodiques. Les occurrences d’élément ne sont pas valides avec ces opérations.           |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.<br/><br/> Voici l’expression XPath de cet élément :  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie la quatrième occurrence d’un élément périodique dont l’identité est 34vswe4.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [RecurringMasterItemId](recurringmasteritemid.md)
- [Opération FindConversation](findconversation-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

