---
title: Conversation (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: L’élément conversation représente une seule conversation.
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458935"
---
# <a name="conversation-conversationtype"></a>Conversation (ConversationType)

L’élément **conversation** représente une seule conversation. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversations](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 **ConversationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |Représente l’identificateur d’une conversation.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Représente la rubrique de conversation. Cet élément est en lecture seule.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contient la liste des destinataires d’une conversation qui a été regroupée à partir d’un dossier particulier. Cet élément est en lecture seule.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contient la liste des destinataires d’une conversation qui est agrégée dans une boîte aux lettres. Cet élément est en lecture seule.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation dans le dossier actif. Cet élément est en lecture seule.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation sur tous les dossiers de la boîte aux lettres.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contient une liste de tous les expéditeurs d’éléments de conversation dans le dossier actif. Cet élément est en lecture seule.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contient une liste de tous les expéditeurs d’éléments de conversation dans la boîte aux lettres.  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |Contient le délai de remise du message qui a été reçu en dernier dans cette conversation dans le dossier actif.  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |Contient le délai de remise du message qui a été reçu en dernier dans cette conversation sur tous les dossiers de la boîte aux lettres.  <br/> |
|[Catégories](categories-ex15websvcsotherref.md) <br/> |Contient une collection de chaînes qui identifient les catégories qui sont appliquées à tous les éléments de conversation dans le dossier actif.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contient la liste des catégories pour tous les éléments de conversation d’une boîte aux lettres.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Contient l’état de l’indicateur agrégé pour les éléments de conversation dans le dossier actif.  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |Contient l’état de l’indicateur agrégé pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Contient une valeur qui indique si au moins un élément de conversation dans le dossier actif a une pièce jointe.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Contient une valeur qui indique si au moins un élément de conversation dans une boîte aux lettres a une pièce jointe.  <br/> |
|[MessageCount](messagecount.md) <br/> |Contient le nombre total d’éléments de conversation dans le dossier actif.  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |Contient le nombre total d’éléments de conversation dans la boîte aux lettres.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Contient le nombre d’éléments de conversation non lus dans un dossier.  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |Contient le décompte de tous les éléments de conversation non lus dans la boîte aux lettres.  <br/> |
|[Taille](size.md) <br/> |Contient la taille de la conversation calculée à partir de la taille de tous les éléments de conversation dans le dossier actif.  <br/> |
|[GlobalSize](globalsize.md) <br/> |Contient la taille de la conversation calculée à partir de la taille de tous les éléments de conversation dans la boîte aux lettres.  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |Contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans le dossier actif.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans une boîte aux lettres.  <br/> |
|[Importance](importance.md) <br/> |Contient l’importance regroupée pour tous les éléments de conversation dans le dossier actif.  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |Contient l’importance regroupée pour tous les éléments de conversation d’une boîte aux lettres.  <br/> |
|[ItemIds](itemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans le dossier actif.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conversations](conversations-ex15websvcsotherref.md) <br/> |Contient un tableau des conversations qui sont renvoyées dans la réponse **FindConversation** .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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



[FindConversation Operation](findconversation-operation.md)
  
[Opération de ApplyConversationAction](applyconversationaction-operation.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

