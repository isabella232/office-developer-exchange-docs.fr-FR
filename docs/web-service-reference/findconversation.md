---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: L’élément FindConversation définit une demande de recherche de conversations dans une boîte aux lettres.
ms.openlocfilehash: e48e0d9fd71dac12fe6848031b2c056ea9a913ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535169"
---
# <a name="findconversation"></a>FindConversation

**L’élément FindConversation** définit une demande de recherche de conversations dans une boîte aux lettres. 
  
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
|Traversée  <br/> |Identifie les types de traversée de sous-arborescence. Cet attribut est facultatif.  <br/> |
|ViewFilter  <br/> |Identifie les filtres d’affichage des types. Cet attribut est facultatif.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut traversal

****

|**Valeur**|**Description**|
|:-----|:-----|
|Superficiel  <br/> |Indique une traversée superficiel.  <br/> |
|Deep  <br/> |Indique une traversée profonde.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valeurs d’attribut ViewFilter

****

|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Recherchez toutes les conversations.  <br/> |
|Marqué d’un indicateur  <br/> |Recherchez les conversations marquées.  <br/> |
|HasAttachment  <br/> |Rechercher des conversations avec des pièces jointes.  <br/> |
|ToOrCcMe  <br/> |Recherchez les conversations qui m’ont été adressées ou cc’d.  <br/> |
|Non lus  <br/> |Recherchez les conversations non lues.  <br/> |
|TaskActive  <br/> |Rechercher les tâches actives.  <br/> |
|TaskOverdue  <br/> |Rechercher les tâches en retard.  <br/> |
|TaskCompleted  <br/> |Rechercher les tâches terminées.  <br/> |
|NoClutter  <br/> |À usage interne uniquement.  <br/> |
|Courrier non trié  <br/> |À usage interne uniquement.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Décrit comment les informations de conversation pagyée sont renvoyées.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Spécifie la condition utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, le nombre maximal d’entrées à renvoyer et les instructions de recherche pour une recherche **FindItem** ou **FindConversation.**  <br/> |
|[SortOrder](sortorder.md) <br/> |Définit le tri des éléments dans une [demande d’opération FindConversation.](findconversation-operation.md) La **propriété conversation:LastDeliveryTime** est la seule propriété prise en charge pour le tri lorsque l’opération **FindConversation** est utilisée.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier à rechercher pour les conversations.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Spécifie si une recherche ou une extraction d’une conversation doit englober la boîte aux lettres principale, la boîte aux lettres d’archivage ou la boîte aux lettres principale et la boîte aux lettres d’archivage.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Spécifie une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifie le jeu de propriétés à renvoyer dans une [réponse d’opération FindConversation.](findconversation-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

