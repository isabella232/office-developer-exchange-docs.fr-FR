---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: L’élément RecurringMasterItemId identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529881"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

L’élément **RecurringMasterItemId** identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**OccurrenceId** <br/> |Identifie une seule occurrence d’un élément maître périodique. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique d’une occurrence d’un élément maître périodique. En outre, l’élément de gabarit périodique est également identifié, car il et la seule occurrence contiendront la même clé de modification. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément. <br/> <br/> Voici l’expression XPath de cet élément : <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange. <br/> <br/>  Voici les expressions XPath de cet élément :  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie l’élément de forme de base périodique en identifiant l’une de ses occurrences à l’aide de l’identificateur 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [OccurrenceItemId](occurrenceitemid.md)
- [Opération FindConversation](findconversation-operation.md)

