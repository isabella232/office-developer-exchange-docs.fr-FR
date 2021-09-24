---
title: Opération CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: L’opération CreateItem crée des éléments dans la Exchange store.
ms.openlocfilehash: 2aee80d883aa623b8074ecc523d1a45fa71962da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538400"
---
# <a name="createitem-operation"></a>Opération CreateItem

L’opération CreateItem crée des éléments dans la Exchange store.
  
## <a name="using-the-createitem-operation"></a>Utilisation de l’opération CreateItem

Vous pouvez utiliser l’opération CreateItem pour créer les opérations suivantes :
  
- Éléments de calendrier
    
- Messages électroniques
    
- Demandes de réunion
    
- Tâches
    
- Contacts
    
Pour plus d’informations, voir [l’opération CreateItem (élément](createitem-operation-calendar-item.md)de calendrier), [l’opération CreateItem (message électronique),](createitem-operation-email-message.md)l’opération [CreateItem (demande](createitem-operation-meeting-request.md)de réunion), l’opération [CreateItem (tâche)](createitem-operation-task.md)et l’opération [CreateItem (contact).](createitem-operation-contact.md)
  
L’opération CreateItem prend en charge l’utilisation d’objets de réponse. Les objets Response supportent l’acceptation et le rejet des réunions et la gestion des boutons de vote inclus dans un message électronique standard. Le tableau suivant répertorie les objets de réponse qui sont gérés dans l’opération CreateItem.
  
|**Objet Response**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Acceptez une demande de réunion.  <br/> |
|CancelCalendarItem  <br/> |Annuler une réunion. Cela diffère de la suppression de tous les participants, car elle supprime également la réunion pour l’organisateur.  <br/> |
|DeclineItem  <br/> |Refuser une demande de réunion.  <br/> |
|ForwardItem  <br/> |Envoyer une demande de réunion à une autre personne en tant que demande de réunion.  <br/> |
|RemoveItem  <br/> |Supprimer une réunion annulée du calendrier.  <br/> |
|ReplyAllToItem  <br/> |Envoyez un message qui inclut le corps de la demande de réunion d’origine à tous les participants à la réunion.  <br/> |
|ReplyToItem  <br/> |Envoyez un message qui inclut le corps de la demande de réunion d’origine à l’expéditeur de la demande de réunion.  <br/> |
|SendReadReceipt  <br/> |Envoyez une réception de lecture à l’expéditeur de la demande de réunion.  <br/> |
|TentativelyAcceptItem  <br/> |Acceptez provisoirement une demande de réunion.  <br/> |
   
L’opération CreateItem prend également en charge des objets de réunion supplémentaires. Le tableau suivant répertorie les objets supplémentaires que l’opération CreateItem prend en charge.
  
|**Objet Meeting**|**Description**|
|:-----|:-----|
|Message de réunion  <br/> |Représente un message de réunion dans le magasin Exchange de réunion. Il s’agit de l’objet de base pour les autres objets de réunion.  <br/> |
|Demande de réunion  <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|Réponse à une réunion  <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|Annulation de réunion  <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateItem (élément de calendrier)](createitem-operation-calendar-item.md)
  
[Opération CreateItem (Contact)](createitem-operation-contact.md)
  
[Opération CreateItem (courrier électronique)](createitem-operation-email-message.md)
  
[Opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md)
  
[Opération CreateItem (tâche)](createitem-operation-task.md)
  
 **CreateItemType**

