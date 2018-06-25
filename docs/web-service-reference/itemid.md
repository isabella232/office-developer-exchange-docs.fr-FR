---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: L’élément ItemId contient la clé unique identificateur et modification d’un élément dans la banque d’informations Exchange.
ms.openlocfilehash: 9c5d71a23e1e4b77d2a50016aa4d765d872d04cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828157"
---
# <a name="itemid"></a>ItemId

L’élément **ItemId** contient la clé unique identificateur et modification d’un élément dans la banque d’informations Exchange. 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Identifie un élément spécifique dans la banque d’informations Exchange. **ID** respecte la casse ; Par conséquent, les comparaisons entre **l’ID** doivent être la casse ou binaire.  <br/> |
|**ChangeKey** <br/> | Identifie une version spécifique d’un élément. <br/><br/>Un **ChangeKey** est requis pour les scénarios suivants : <br/> <br/>-L’élément [UpdateItem](updateitem.md) requiert un **ChangeKey** si l’attribut **ConflictResolution** est défini sur résoudre automatiquement. Résolution automatique est une valeur par défaut. Si l’attribut **ChangeKey** n’est pas inclus, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorChangeKeyRequired**.  <br/><br/>-L’élément [SendItem](senditem.md) requiert un **ChangeKey** vérifier si l’opération s’agir de la version la plus récente d’un élément. Si l’attribut **ChangeKey** n’est pas inclus dans l' **ID d’élément** , ou si la **ChangeKey** est vide, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement lorsqu’un élément ou un dossier est copié.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement lorsqu’un élément ou un dossier est créé.  <br/> |
|[Supprimer (ItemSync)](delete-itemsync.md) <br/> |Identifie un seul élément à supprimer dans le magasin de client local.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement lorsqu’un élément ou un dossier est supprimé.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande pour exporter un élément de boîte aux lettres unique.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[Ignorer](ignore.md) <br/> |Identifie les éléments à ignorer lors de la synchronisation.  <br/> |
|[Item](item.md) <br/> |Représente un élément Exchange générique.  <br/> |
|[Élément (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un seul élément à télécharger dans une boîte aux lettres.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.  <br/><br/> Vous trouverez ci-dessous l’expression XPath pour cet élément : <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemId](itemids.md) <br/> | Contient l’identité unique des éléments, des éléments d’occurrence et des éléments de gabarit périodiques permet de supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange. <br/> <br/>  Les expressions XPath pour cet élément sont les suivantes : <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[ItemId (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement qui se produit lorsqu’un élément est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement qui se produit lorsqu’un élément est déplacé à partir du dossier parent d’un vers un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement qui est déclenché par un nouvel élément de messagerie dans une boîte aux lettres.  <br/> |
|[Occurrence](occurrence.md) <br/> |Représente une seule occurrence de modification d’un élément de calendrier périodique.  <br/> |
|[PlayOnPhone (Exchange Web Services)](playonphone-exchange-web-services.md) <br/> |Représente une demande de lecture d’un élément sur un téléphone.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[RoomList](roomlist.md) <br/> |Représente une adresse de messagerie qui identifie une liste de salles de réunion.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande pour télécharger un élément de boîte aux lettres unique.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Définit un objet de configuration utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md)
- [Opération UploadItems](uploaditems-operation.md) 
- [FindConversation Operation](findconversation-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

