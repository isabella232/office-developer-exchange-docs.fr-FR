---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: L’élément ItemId contient l’identificateur unique et la clé de modification d’un élément dans la Banque d’Exchange.
localization_priority: Priority
ms.openlocfilehash: d5931702225c6864b1ca60a6f0753b65f65aca30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441561"
---
# <a name="itemid"></a>ItemId

L’élément **ItemId** contient l’identificateur unique et la clé de modification d’un élément dans la Banque d’Exchange. 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Identifie un élément spécifique dans la Banque d’informations Exchange. L' **ID** respecte la casse ; par conséquent, les comparaisons entre les **ID** doivent respecter la casse ou être au format binaire.  <br/> |
|**ChangeKey** <br/> | Identifie une version spécifique d’un élément. <br/><br/>Un **ChangeKey** est requis pour les scénarios suivants : <br/> <br/>-L’élément [UpdateItem](updateitem.md) nécessite un **ChangeKey** si l’attribut **ConflictResolution** est défini sur autosolve. Autosolve est une valeur par défaut. Si l’attribut **ChangeKey** n’est pas inclus, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorChangeKeyRequired**.  <br/><br/>-L’élément [SendItem](senditem.md) nécessite un **ChangeKey** pour tester si l’opération tentée agira sur la version la plus récente d’un élément. Si l’attribut **ChangeKey** n’est pas inclus dans l' **ItemId** ou si **ChangeKey** est vide, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement lors de la copie d’un élément ou d’un dossier.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Représente un événement lors de la création d’un élément ou d’un dossier.  <br/> |
|[Supprimer (ItemSync)](delete-itemsync.md) <br/> |Identifie un élément unique à supprimer dans le magasin client local.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Représente un événement lors de la suppression d’un élément ou d’un dossier.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande d’exportation d’un seul élément de boîte aux lettres.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Représente la première occurrence d’un élément de calendrier périodique.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[Ignore](ignore.md) <br/> |Identifie les éléments à ignorer lors de la synchronisation.  <br/> |
|[Élément](item.md) <br/> |Représente un élément Exchange générique.  <br/> |
|[Élément (UploadItemType)](item-uploaditemtype.md) <br/> |Représente un élément unique à télécharger dans une boîte aux lettres.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contient un identificateur d’élément et les mises à jour à appliquer à l’élément.  <br/><br/> Voici l’expression XPath de cet élément : <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange. <br/> <br/>  Voici les expressions XPath de cet élément : <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[ItemIds (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Représente la dernière occurrence d’un élément de calendrier périodique.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Représente un événement qui se produit lorsqu’un élément est modifié.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Représente un événement qui se produit lorsqu’un élément est déplacé d’un dossier parent à un autre dossier parent.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.  <br/> |
|[Réunions](occurrence.md) <br/> |Représente une occurrence modifiée unique d’un élément de calendrier périodique.  <br/> |
|[PlayOnPhone (services Web Exchange)](playonphone-exchange-web-services.md) <br/> |Représente une demande de lecture d’un élément sur un téléphone.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[RoomList](roomlist.md) <br/> |Représente une adresse de messagerie qui identifie une liste de salles de réunion.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contient l’État et les résultats d’une demande de téléchargement d’un seul élément de boîte aux lettres.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Définit un objet de configuration utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExportItems](exportitems-operation.md)
- [Opération UploadItems](uploaditems-operation.md) 
- [Opération FindConversation](findconversation-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

