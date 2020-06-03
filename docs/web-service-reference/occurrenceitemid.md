---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: L’élément OccurrenceItemId identifie une seule occurrence d’un élément périodique.
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468375"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

L’élément **OccurrenceItemId** identifie une seule occurrence d’un élément périodique. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Identifie le masque périodique d’un élément périodique. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique de l’occurrence de la page maître périodique ou d’un élément. Si la forme de base périodique ou l’une de ses occurrences change, le **ChangeKey** change. Le **ChangeKey** est le même pour le masque périodique et toutes les occurrences.  <br/> |
|**InstanceIndex** <br/> |Identifie l’index de l’occurrence de l’élément. Cet attribut est obligatoire. Cette valeur représente un entier.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemIds](itemids.md) <br/> | Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange. <br/><br/>Voici les expressions XPath de cet élément : <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**Remarque**: l’opération [MoveItem](moveitem-operation.md) et l' [opération CopyItem](copyitem-operation.md) fonctionnent uniquement avec des éléments de calendrier uniques et des éléments de forme de base périodiques. Les occurrences d’élément ne sont pas valides avec ces opérations.           |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.<br/><br/> Voici l’expression XPath de cet élément :  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie la quatrième occurrence d’un élément périodique ayant l’identité 34vswe4.
  
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

