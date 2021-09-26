---
title: DraftItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c228f7e7-6dc8-476d-9b8c-99cd5b6f9f0c
description: L’élément DraftItemIds contient un tableau d’identificateurs d’éléments pour les éléments de brouillon dans une conversation.
ms.openlocfilehash: 9c114e509418138d442ae2cf20278cda410bf9dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541440"
---
# <a name="draftitemids"></a>DraftItemIds

**L’élément DraftItemIds** contient un tableau d’identificateurs d’éléments pour les éléments de brouillon dans une conversation. 
  
```XML
<DraftItemIds>
   <ItemId/>
   <OccirrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</DraftItemIds>
```

 **NonEmptyArrayOfBaseItemIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemid.md)  |  [OccurrenceItemId](occurrenceitemid.md)  |  [RecurringMasterItemId](recurringmasteritemid.md)  |  [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)
  
### <a name="parent-elements"></a>Éléments parents

[Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

