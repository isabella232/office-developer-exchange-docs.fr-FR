---
title: Opération CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: L’opération CreateItem crée des éléments dans la Banque d’Exchange.
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458865"
---
# <a name="createitem-operation"></a>Opération CreateItem

L’opération CreateItem crée des éléments dans la Banque d’Exchange.
  
## <a name="using-the-createitem-operation"></a>Utilisation de l’opération CreateItem

Vous pouvez utiliser l’opération CreateItem pour créer les éléments suivants :
  
- Éléments de calendrier
    
- Messages électroniques
    
- Demandes de réunion
    
- Tâches
    
- Contacts
    
Pour plus d’informations, consultez opération [CreateItem (élément de calendrier)](createitem-operation-calendar-item.md), [opération CreateItem (message électronique)](createitem-operation-email-message.md), [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md), [opération CreateItem (tâche)](createitem-operation-task.md)et [opération CreateItem (contact)](createitem-operation-contact.md).
  
L’opération CreateItem prend en charge l’utilisation des objets Response. Les objets Response prennent en charge l’acceptation et le rejet des réunions et la gestion des boutons de vote inclus dans un message électronique standard. Le tableau suivant répertorie les objets Response qui sont gérés dans l’opération CreateItem.
  
|**Response, objet**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Accepter une demande de réunion.  <br/> |
|CancelCalendarItem  <br/> |Annuler une réunion. Cela diffère de la suppression de tous les participants, car elle supprime également la réunion pour l’organisateur.  <br/> |
|DeclineItem  <br/> |Refuser une demande de réunion.  <br/> |
|ForwardItem  <br/> |Envoyer une demande de réunion à une autre personne sous la forme d’une demande de réunion.  <br/> |
|RemoveItem  <br/> |Supprimer une réunion annulée du calendrier.  <br/> |
|ReplyAllToItem  <br/> |Envoyer un message qui inclut le corps de la demande de réunion d’origine à tous les participants de la réunion.  <br/> |
|ReplyToItem  <br/> |Envoyez un message qui inclut le corps de la demande de réunion d’origine à l’expéditeur de la demande de réunion.  <br/> |
|SendReadReceipt  <br/> |Envoyer une confirmation de lecture à l’expéditeur de la demande de réunion.  <br/> |
|TentativelyAcceptItem  <br/> |Accepter provisoirement une demande de réunion.  <br/> |
   
L’opération CreateItem prend également en charge des objets de réunion supplémentaires. Le tableau suivant répertorie les objets supplémentaires pris en charge par l’opération CreateItem.
  
|**Objet de réunion**|**Description**|
|:-----|:-----|
|Message de réunion  <br/> |Représente un message de réunion dans la Banque d’aide Exchange. Il s’agit de l’objet de base pour les autres objets de réunion.  <br/> |
|Demande de réunion  <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|Réponse à une réunion  <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|Annulation de réunion  <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateItem (élément de calendrier)](createitem-operation-calendar-item.md)
  
[Opération CreateItem (contact)](createitem-operation-contact.md)
  
[Opération CreateItem (message électronique)](createitem-operation-email-message.md)
  
[Opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md)
  
[Opération CreateItem (tâche)](createitem-operation-task.md)
  
 **CreateItemType**

