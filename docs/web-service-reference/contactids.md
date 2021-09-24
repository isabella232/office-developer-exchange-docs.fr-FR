---
title: ContactIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c444f818-412b-41ac-9523-50246e50eae0
description: L’élément ContactIds contient un tableau d’identificateurs d’élément de contact.
ms.openlocfilehash: 05c26af6dc1a5b826025e4145116d3df5eee8d62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529216"
---
# <a name="contactids"></a>ContactIds

**L’élément ContactIds** contient un tableau d’identificateurs d’élément de contact. 
  
```XML
<ContactIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</ContactIds>
```

 **NonEmptyArrayOfBaseItemIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemid.md)  |  [OccurrenceItemId](occurrenceitemid.md)  |  [RecurringMasterItemId](recurringmasteritemid.md)  |  [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetImItems](getimitems.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

