---
title: CreateItem Operation
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
description: L’opération CreateItem crée des éléments dans la banque d’informations Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755723"
---
# <a name="createitem-operation"></a>CreateItem Operation

L’opération CreateItem crée des éléments dans la banque d’informations Exchange.
  
## <a name="using-the-createitem-operation"></a>Utilisation de l’opération CreateItem

Vous pouvez utiliser l’opération CreateItem pour créer les éléments suivants :
  
- Éléments de calendrier
    
- Messages électroniques
    
- Demandes de rendez-vous
    
- Tâches
    
- Contacts
    
Pour plus d’informations, voir [CreateItem operation (élément de calendrier)](createitem-operation-calendar-item.md), [opération CreateItem (e-mail)](createitem-operation-email-message.md), [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md), [opération CreateItem (tâche)](createitem-operation-task.md)et [opération CreateItem (contacts) ](createitem-operation-contact.md).
  
L’opération CreateItem prend en charge l’utilisation d’objets de réponse. Objets de réponse prennent en charge l’acceptation et le rejet des réunions et la gestion des boutons de vote qui sont inclus dans un message électronique standard. Le tableau suivant répertorie les objets de réponse qui sont gérées de l’opération CreateItem.
  
|**Objet de réponse**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Accepter une demande de réunion.  <br/> |
|CancelCalendarItem  <br/> |Annuler une réunion. Cela diffère de la suppression de tous les participants, car il supprime la réunion pour l’organisateur également.  <br/> |
|DeclineItem  <br/> |Refuser une demande de réunion.  <br/> |
|ForwardItem  <br/> |Envoyer une demande de réunion à une autre personne en tant qu’une demande de réunion.  <br/> |
|RemoveItem  <br/> |Supprimer une réunion annulée à partir du calendrier.  <br/> |
|ReplyAllToItem  <br/> |Envoyer un message qui inclut le corps de la demande de réunion d’origine à tous les participants de la réunion.  <br/> |
|ReplyToItem  <br/> |Envoyer un message qui inclut le corps de la demande de réunion d’origine à l’expéditeur de la demande de réunion.  <br/> |
|SendReadReceipt  <br/> |Envoyer une confirmation de lecture à l’expéditeur de la demande de réunion.  <br/> |
|TentativelyAcceptItem  <br/> |Accepter provisoirement une demande de réunion.  <br/> |
   
L’opération CreateItem prend également en charge les objets de la conférence supplémentaires. Le tableau suivant répertorie les objets supplémentaires que l’opération CreateItem prend en charge.
  
|**Objet de la réunion**|**Description**|
|:-----|:-----|
|Message de réunion  <br/> |Représente un message de réunion dans la banque d’informations Exchange. Il s’agit de l’objet de base pour les autres objets de la réunion.  <br/> |
|Demande de réunion  <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|Réponse à une réunion  <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|Annulation de réunion  <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateItem (élément de calendrier)](createitem-operation-calendar-item.md)
  
[Opération CreateItem (contacts)](createitem-operation-contact.md)
  
[Opération CreateItem (e-mail)](createitem-operation-email-message.md)
  
[Opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md)
  
[Opération CreateItem (tâche)](createitem-operation-task.md)
  
 **CreateItemType**

