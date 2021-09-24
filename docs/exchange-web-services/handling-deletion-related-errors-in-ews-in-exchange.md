---
title: Gestion des erreurs liées à la suppression dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Découvrez comment gérer les erreurs liées à la suppression dans les applications que vous développez à l’aide de l’API manaëlle EWS ou EWS dans Exchange.
ms.openlocfilehash: d82901a2ebc8577258e191cbd014db93cc40d099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513254"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la suppression dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la suppression dans les applications que vous développez à l’aide de l’API manaëlle EWS ou EWS dans Exchange.
  
Si votre application [supprime des éléments et des dossiers,](deleting-items-by-using-ews-in-exchange.md)vous de devez peut-être gérer les erreurs liées à la suppression. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS.
  
**Tableau 1 : Erreurs liées à la suppression et comment les gérer**

|**Erreur**|**Se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Supprimez une instance d’une tâche périodique et la **propriété AffectedTaskOccurrence** n’est pas définie.  <br/> |Définition de **la propriété AffectedTaskOccurrence** et nouvelle tentative de suppression.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Mettez à jour un élément de calendrier situé dans le dossier Éléments supprimés lorsque la mise à jour entraîne l’envoi d’une invitation à une réunion aux participants.  <br/> |Annulation de la mise à jour ou déplacement de l’élément de calendrier vers le dossier Calendrier par défaut et mise à jour de l’élément de calendrier.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Référencer une occurrence supprimée d’un rendez-vous périodique.  <br/> |Suppression d’une référence à une occurrence supprimée.  <br/> |
|ErrorCannotDeleteObject  <br/> |Supprimez un élément qui ne peut pas être supprimé.  <br/> |Abandon des tentatives de suppression de l’élément.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Supprimez une occurrence d’une tâche non périodique ou supprimez la dernière occurrence d’une tâche périodique.  <br/> |La suppression d’une tâche non périodique ou l’arrêt des tentatives de suppression de la dernière occurrence d’une tâche périodique.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Supprimez un dossier spécifique.  <br/> |Indiquant que les dossiers par défaut ne peuvent pas être supprimés.  <br/> |
|ErrorItemNotFound  <br/> |Accéder à un élément supprimé définitivement.  <br/> |Suppression des références à un élément lorsqu’il est supprimé du store. Si un élément est récupéré, veillez à rétablir les références requises au client.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Supprimez un élément de calendrier sans spécifier si des annulations de réunion doivent être envoyées.  <br/> |Spécifier que les annulations de réunion doivent ou ne doivent pas être envoyées.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Notifications de pull pour les événements de boîte aux lettres liés à la suppression d’EWS dans Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

