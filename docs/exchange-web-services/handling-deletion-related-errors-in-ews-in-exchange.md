---
title: Gestion des erreurs liées aux suppression dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Découvrez comment gérer les erreurs liées aux suppression dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 0dc16c3350bb75fb1e91650f0a0f0b7423727eeb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754771"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées aux suppression dans EWS dans Exchange

Découvrez comment gérer les erreurs liées aux suppression dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Si votre application [supprime les éléments et les dossiers](deleting-items-by-using-ews-in-exchange.md), vous devrez peut-être gérer les erreurs liées à la suppression. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS.
  
**Tableau 1 : Erreurs liées à la suppression et comment les gérer**

|**Erreur**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Supprimer une instance d’une tâche périodique, et la propriété **AffectedTaskOccurrence** n’est pas définie.  <br/> |Définition de la propriété **AffectedTaskOccurrence** et la suppression de nouvelle tentative en cours.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Mettre à jour un élément de calendrier situé dans le dossier éléments supprimés lors de la mise à jour risque de l’envoi d’une invitation à la réunion aux participants.  <br/> |L’annulation de la mise à jour ou déplaçant l’élément de calendrier dans le dossier de calendrier par défaut et mise à jour de l’élément de calendrier.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Faire référence à une occurrence d’un rendez-vous périodique supprimée.  <br/> |Suppression d’une référence à une occurrence supprimée.  <br/> |
|ErrorCannotDeleteObject  <br/> |Supprimer un élément qui ne peut pas être supprimé.  <br/> |Quitter tente de supprimer l’élément.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Supprimer une occurrence d’une tâche non périodique ou la dernière occurrence d’une tâche périodique.  <br/> |Suppression d’une tâche non périodique ou quitter tente de supprimer la dernière occurrence d’une tâche périodique.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Supprimer un dossier unique.  <br/> |Indiquant que les dossiers par défaut ne peut pas être supprimées.  <br/> |
|ErrorItemNotFound  <br/> |Accéder à un élément définitivement supprimé.  <br/> |Suppression des références à un élément lorsqu’il est supprimé de la banque. Si un élément est récupéré, assurez-vous que vous rétablissez les références requises pour le client.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Supprimer un élément de calendrier sans spécifier si les annulations de réunion doivent être envoyées.  <br/> |Vous spécifiez que les annulations de réunion doit ou ne doit pas être envoyée.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Extraction des notifications pour les événements liés à la suppression de boîte aux lettres EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

