---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: L’élément RecurringMasterItemId identifie un élément récurrence maître en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.
ms.openlocfilehash: d00794f2b5b1893e1829a3f09df9f3e88266964d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523628"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

**L’élément RecurringMasterItemId** identifie un élément récurrence maître en identifiant les identificateurs de l’un de ses éléments d’occurrence associés. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**OccurrenceId** <br/> |Identifie une occurrence unique d’un élément principal périodique. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique d’une occurrence unique d’un élément principal périodique. En outre, l’élément maître périodique est également identifié car il et l’occurrence unique contiendra la même touche de modification. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’éléments pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément. <br/> <br/> Voici l’expression XPath de cet élément : <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contient les identités uniques des éléments, des éléments d’occurrence et des éléments maîtres périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Exchange store. <br/> <br/>  Les expressions XPath de cet élément sont les suivantes :  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie l’élément principal périodique en identifiant l’une de ses occurrences avec l’identificateur 56lkjh6.
  
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

