---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: L’élément ConversationAction contient une seule action à appliquer à une même conversation.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755637"
---
# <a name="conversationaction"></a>ConversationAction

L’élément **ConversationAction** contient une seule action à appliquer à une même conversation. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Action (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) . Cet élément doit être présent.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contient l’identificateur de la conversation qui auront l’action spécifiée par l’élément [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) appliqué aux éléments de la conversation. Cet élément doit être présent.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, suppression, déplacement et en définissant l’état de lecture sur les éléments de conversation dans un dossier cible.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Contient la date et l’heure de dernière synchronisation une conversation. Cet élément doit être présent lorsque vous tentez de supprimer tous les éléments qui ont été reçus jusqu'à l’heure spécifiée dans une conversation.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Indique si la réponse est envoyée dès que l’action démarre le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée. Cet élément doit être présent pour la réponse à envoyer asynchrone à l’action demandée.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination de copie et les actions de déplacement.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient une collection de chaînes qui identifient les catégories auquel appartiennent les éléments dans une conversation.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Spécifie un indicateur qui permet la suppression de tous les nouveaux éléments dans une conversation.  <br/> |
|[Estlu](isread.md) <br/> |Indique si un message a été lu.  <br/> |
|[DeleType](deletetype.md) <br/> |Indique comment les éléments dans une conversation sont supprimés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Contient une collection des conversations et les actions à appliquer à leur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

**Valeurs de texte des éléments ConversationAction**

|**Valeur**|**Description**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Toujours classer la conversation.  <br/> |
|AlwaysDelete  <br/> |Toujours supprimer la conversation.  <br/> |
|AlwaysMove  <br/> |Toujours déplacer la conversation.  <br/> |
|Suppression  <br/> |Supprimer la conversation.  <br/> |
|Déplacer  <br/> |Déplacer la conversation.  <br/> |
|Copier  <br/> |Copiez la conversation.  <br/> |
|SetReadState  <br/> |Définir l’état de lecture de la conversation.  <br/> |
|SetRetentionPolicy  <br/> |Définir la stratégie de rétention pour la conversation.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de ApplyConversationAction](applyconversationaction-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

