---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: L’élément FindConversation définit une requête pour rechercher des conversations dans une boîte aux lettres.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462646"
---
# <a name="findconversation"></a>FindConversation

L’élément **FindConversation** définit une requête pour rechercher des conversations dans une boîte aux lettres. 
  
[FindConversation](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 **FindConversationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

****

|**Attribut**|**Description**|
|:-----|:-----|
|Traversée  <br/> |Identifie les types de parcours de sous-arborescence. Cet attribut est facultatif.  <br/> |
|ViewFilter  <br/> |Identifie les filtres d’affichage de types. Cet attribut est facultatif.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut transversal

****

|**Valeur**|**Description**|
|:-----|:-----|
|Partielle  <br/> |Indique un parcours superficiel.  <br/> |
|Développée  <br/> |Indique un parcours approfondi.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valeurs d’attribut ViewFilter

****

|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Rechercher toutes les conversations.  <br/> |
|Marqué d’un indicateur  <br/> |Rechercher des conversations avec indicateur.  <br/> |
|HasAttachment  <br/> |Rechercher des conversations avec des pièces jointes.  <br/> |
|ToOrCcMe  <br/> |Rechercher les conversations adressées ou CC avec moi.  <br/> |
|Non lus  <br/> |Rechercher des conversations non lues.  <br/> |
|TaskActive  <br/> |Rechercher des tâches actives.  <br/> |
|TaskOverdue  <br/> |Recherchez les tâches en retard.  <br/> |
|TaskCompleted  <br/> |Recherchez les tâches terminées.  <br/> |
|Nodésordre  <br/> |À usage interne uniquement.  <br/> |
|Courrier non trié  <br/> |À usage interne uniquement.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Indique comment les informations de conversation paginée sont renvoyées.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Spécifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et l’orientation de la recherche pour une recherche **FindItem** ou **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Définit le mode de tri des éléments dans une demande d' [opération FindConversation](findconversation-operation.md) . La propriété **conversation : LastDeliveryTime** est la seule propriété prise en charge pour le tri lorsque l’opération **FindConversation** est utilisée.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier dans lequel Rechercher des conversations.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Indique si une recherche ou une récupération d’une conversation doit s’étendre sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Spécifie une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifie le jeu de propriétés à renvoyer dans une réponse d' [opération FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

