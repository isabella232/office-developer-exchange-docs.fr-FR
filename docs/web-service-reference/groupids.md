---
title: GroupID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4d32cb3b-eb84-4816-89cd-26dcf5131bc8
description: L’élément les GroupID identifie un tableau d’identificateurs de groupe de messagerie instantanée.
ms.openlocfilehash: 0e463a3a74eb3a4996b521f77e1175913b22d16b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827763"
---
# <a name="groupids"></a>GroupID

L’élément **les GroupID** identifie un tableau d’identificateurs de groupe de messagerie instantanée. 
  
```XML
<GroupIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</GroupIds>
```

 **NonEmptyArrayOfBaseItemIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetImItems](getimitems.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

