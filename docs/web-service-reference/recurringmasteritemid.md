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
description: L’élément RecurringMasterItemId identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829015"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

L’élément **RecurringMasterItemId** identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ID d’occurrence** <br/> |Identifie une seule occurrence d’un rendez-vous périodique. Cet attribut est requis.  <br/> |
|**ChangeKey** <br/> |Identifie une version spécifique d’une seule occurrence d’un rendez-vous périodique. En outre, le rendez-vous périodique est également identifié, car elle et l’occurrence contiendra la même clé change. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément. <br/> <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément : <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemId](itemids.md) <br/> | Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange. <br/> <br/>  Les expressions XPath pour cet élément sont les suivantes :  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant identifie le rendez-vous périodique en identifiant une de ses occurrences avec l’identificateur 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [OccurrenceItemId](occurrenceitemid.md)
- [FindConversation Operation](findconversation-operation.md)

