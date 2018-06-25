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
description: L’élément FindConversation définit une requête pour rechercher les conversations dans une boîte aux lettres.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756381"
---
# <a name="findconversation"></a>FindConversation

L’élément **FindConversation** définit une requête pour rechercher les conversations dans une boîte aux lettres. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

****

|**Attribut**|**Description**|
|:-----|:-----|
|Traversée du contenu  <br/> |Identifie les types de parcours sous-arborescence. Cet attribut est facultatif.  <br/> |
|AffichageFiltrer  <br/> |Identifie les filtres d’affichage types. Cet attribut est facultatif.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut Traversal

****

|**Valeur**|**Description**|
|:-----|:-----|
|Peu profond  <br/> |Indique un parcours en surface.  <br/> |
|Profond  <br/> |Indique un parcours en profondeur.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valeurs des attributs AffichageFiltrer

****

|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Recherchez toutes les conversations.  <br/> |
|Marqué d’un indicateur  <br/> |Rechercher les conversations avec indicateur.  <br/> |
|HasAttachment  <br/> |Rechercher les conversations avec les pièces jointes.  <br/> |
|ToOrCcMe  <br/> |Rechercher les conversations adressé ou cc serait Me.  <br/> |
|Unread  <br/> |Rechercher les conversations non lues.  <br/> |
|TaskActive  <br/> |Rechercher des tâches actives.  <br/> |
|TaskOverdue  <br/> |Rechercher les tâches en retard.  <br/> |
|TaskCompleted  <br/> |Rechercher les tâches terminées.  <br/> |
|NoClutter  <br/> |Réservé à un usage interne  <br/> |
|Encombrement  <br/> |Réservé à un usage interne  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Décrit comment paginée conversation les informations sont retournées.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Spécifie la condition qui sert à identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Définit comment les éléments sont triés dans une requête [d’opération FindConversation](findconversation-operation.md) . La propriété **conversation : LastDeliveryTime** est la seule propriété qui est pris en charge pour le tri lors de l’opération **FindConversation** est utilisée.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier pour rechercher des conversations.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Spécifie si une recherche ou extraction d’une conversation doit couvrir la boîte aux lettres principale, boîte aux lettres d’archivage ou les deux principal et archiver des boîtes aux lettres.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Spécifie une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifie la propriété définie pour retourner une réponse de [l’opération FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[FindConversation Operation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

