---
title: Gestion des erreurs liées à la suppression dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Découvrez comment gérer les erreurs liées à la suppression dans les applications que vous développez à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 41c217c1c3815606d898b8237ea327f34869174b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455946"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la suppression dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la suppression dans les applications que vous développez à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Si votre application [supprime des éléments et des dossiers](deleting-items-by-using-ews-in-exchange.md), il se peut que vous deviez gérer les erreurs liées à la suppression. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS.
  
**Tableau 1 : erreurs liées à la suppression et comment les gérer**

|**Error**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Supprimer une instance d’une tâche périodique, et la propriété **AffectedTaskOccurrence** n’est pas définie.  <br/> |Définition de la propriété **AffectedTaskOccurrence** et nouvelle tentative de suppression.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Mettre à jour un élément de calendrier situé dans le dossier éléments supprimés lorsque la mise à jour entraînerait l’envoi d’une invitation à une réunion aux participants.  <br/> |Annuler la mise à jour ou de replacer l’élément de calendrier dans le dossier calendrier par défaut et mettre à jour l’élément de calendrier.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Faire référence à une occurrence supprimée d’un rendez-vous périodique.  <br/> |Suppression d’une référence à une occurrence supprimée.  <br/> |
|ErrorCannotDeleteObject  <br/> |Supprimer un élément qui ne peut pas être supprimé.  <br/> |Quitter les tentatives de suppression de l’élément.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Supprimer une occurrence d’une tâche non périodique ou supprimer la dernière occurrence d’une tâche périodique.  <br/> |Suppression d’une tâche périodique ou abandon des tentatives de suppression de la dernière occurrence d’une tâche périodique.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Supprimez un dossier unique.  <br/> |Indiquant que les dossiers par défaut ne peuvent pas être supprimés.  <br/> |
|ErrorItemNotFound  <br/> |Accéder à un élément supprimé définitivement.  <br/> |Suppression des références à un élément lorsqu’il est supprimé de la Banque. Si un élément est récupéré, veillez à rétablir les références requises sur le client.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Supprimer un élément de calendrier sans indiquer si les annulations de réunion doivent être envoyées.  <br/> |Spécifier que les annulations de réunion doivent ou ne doivent pas être envoyées.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Notifications de type pull pour les événements de boîte aux lettres liés à la suppression EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

