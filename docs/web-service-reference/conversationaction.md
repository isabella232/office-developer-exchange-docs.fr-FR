---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: L’élément ConversationAction contient une seule action à appliquer à une seule conversation.
ms.openlocfilehash: 04af68b4ad8442160792fd3aa9f3259058a0f3a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531105"
---
# <a name="conversationaction"></a>ConversationAction

**L’élément ConversationAction** contient une seule action à appliquer à une seule conversation. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 **ConversationActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Action (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Contient l’action à effectuer sur la conversation spécifiée par [l’élément ConversationId.](conversationid.md) Cet élément doit être présent.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contient l’identificateur de la conversation qui aura l’action spécifiée par [l’élément Action (ConversationActionTypeType)](action-conversationactiontypetype.md) appliqué aux éléments de la conversation. Cet élément doit être présent.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, de la suppression, du déplacement et de la définition de l’état de lecture sur les éléments de conversation dans un dossier cible.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Contient la date et l’heure de la dernière synchronisation d’une conversation. Cet élément doit être présent lors de la tentative de suppression de tous les éléments d’une conversation reçus jusqu’à l’heure spécifiée.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Indique si la réponse est envoyée dès que l’action démarre le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée. Cet élément doit être présent pour que la réponse soit envoyée asynchrone à l’action demandée.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination pour les actions de copie et de déplacement.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient une collection de chaînes qui identifient les catégories à laquelle appartiennent les éléments d’une conversation.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Spécifie un indicateur qui permet la suppression de tous les nouveaux éléments d’une conversation.  <br/> |
|[IsRead](isread.md) <br/> |Indique si un message a été lu.  <br/> |
|[DeleteType](deletetype.md) <br/> |Indique comment les éléments d’une conversation sont supprimés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Contient une collection de conversations et les actions à leur appliquer.  <br/> |
   
## <a name="text-value"></a>Valeur texte

**Valeurs de texte de l’élément ConversationAction**

|**Valeur**|**Description**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Catégoriser toujours la conversation.  <br/> |
|AlwaysDelete  <br/> |Supprimez toujours la conversation.  <br/> |
|AlwaysMove  <br/> |Déplacez toujours la conversation.  <br/> |
|Supprimer  <br/> |Supprimez la conversation.  <br/> |
|Move  <br/> |Déplacez la conversation.  <br/> |
|Copy  <br/> |Copiez la conversation.  <br/> |
|SetReadState  <br/> |Définissez l’état de lecture de la conversation.  <br/> |
|SetRetentionPolicy  <br/> |Définissez la stratégie de rétention pour la conversation.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de ApplyConversationAction](applyconversationaction-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

