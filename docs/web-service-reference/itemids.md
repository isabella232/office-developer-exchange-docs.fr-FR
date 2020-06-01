---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: L’élément ItemIds contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460602"
---
# <a name="itemids"></a>ItemIds
  
L’élément **ItemIds** contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents. 
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifie une seule occurrence d’un élément périodique.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifie un élément de la forme de base de récurrence en identifiant l’un de ses éléments d’occurrences associés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Représente une conversation unique.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Définit une demande de suppression d’éléments dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Élément racine qui définit une demande d’envoi d’éléments dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Définit une demande d’obtention d’éléments à partir de la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’éléments dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Définit une demande de copie des éléments dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteItem](deleteitem-operation.md)
- [Opération SendItem](senditem-operation.md) 
- [Opération GetItem](getitem-operation.md)
- [Opération MoveItem](moveitem-operation.md)
- [Opération CopyItem](copyitem-operation.md)
- [Opération FindConversation](findconversation-operation.md)

