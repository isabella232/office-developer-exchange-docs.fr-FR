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
ms.openlocfilehash: e3d7b6efc49775f54219ce0dc0ec39a34a95f8fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828639"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

L’élément **OccurrenceItemId** identifie une seule occurrence d’un élément périodique. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Identifie le contrôleur périodique d’un élément périodique. Cet attribut est requis.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique de la forme de base périodique ou une occurrence de l’élément. Si la forme de base périodique ou une de ses occurrences changent, le **ChangeKey** change. Le **ChangeKey** est la même pour le contrôleur périodique et toutes les occurrences.  <br/> |
|**InstanceIndex** <br/> |Identifie l’index de l’occurrence de l’élément. Cet attribut est requis. Cette valeur représente un entier.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemId](itemids.md) <br/> | Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange. <br/><br/>Les expressions XPath pour cet élément sont les suivantes : <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**Remarque**: [MoveItem](moveitem-operation.md) et [les opérations CopyItem](copyitem-operation.md) ne fonctionnent qu’avec les éléments de calendrier et les éléments périodiques. Occurrences d’élément ne sont pas valides avec ces opérations.           |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.<br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie l’occurrence d’un élément périodique ayant l’identité 34vswe4 quatrième.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [RecurringMasterItemId](recurringmasteritemid.md)
- [FindConversation Operation](findconversation-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

