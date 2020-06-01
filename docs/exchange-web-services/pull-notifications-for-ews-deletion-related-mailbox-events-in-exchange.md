---
title: Notifications de type pull pour les événements de boîte aux lettres liés à la suppression EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Découvrez les événements de boîte aux lettres déclenchés lorsque vous supprimez des éléments à l’aide d’EWS dans Exchange.
ms.openlocfilehash: c3d98ff798e3d0f6d214111d51da2c81278fd17d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457654"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Notifications de type pull pour les événements de boîte aux lettres liés à la suppression EWS dans Exchange

Découvrez les événements de boîte aux lettres déclenchés lorsque vous supprimez des éléments à l’aide d’EWS dans Exchange.
  
Lorsque vous [supprimez des éléments et des dossiers d’une boîte aux lettres](deleting-items-by-using-ews-in-exchange.md), un événement de boîte aux lettres est déclenché. Différentes versions d’Exchange renvoient des événements de boîte aux lettres différents en réponse à des modifications apportées aux éléments et aux dossiers d’une boîte aux lettres. Le tableau suivant identifie les événements de boîte aux lettres renvoyés pour les suppressions lorsque vous utilisez des notifications de type pull pour vous abonner à des événements de boîte aux lettres. 
  
**Tableau 1 : événements de boîte aux lettres liés à la suppression pour les notifications de type pull**

|**Type de suppression et opération EWS**|**Notification Exchange 2010 lorsque vous spécifiez chaque identificateur de dossier**|**Notification Exchange 2010 lorsque vous spécifiez tous les dossiers**|**Notification Exchange Online et Exchange 2013 lorsque vous spécifiez chaque identificateur de dossier**|**Exchange Online et Exchange 2013 lorsque vous spécifiez tous les dossiers**|
|:-----|:-----|:-----|:-----|:-----|
|Suppression douce via l' [opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |MovedEvent pour l’élément. Cette énumération spécifie à la fois les anciens et nouveaux identificateurs de dossiers parents. L’élément est déplacé vers le dossier des suppressions dans la benne.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément à partir du dossier de recherche AllItems par défaut.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Suppression définitive via l' [opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément à partir du dossier de recherche AllItems par défaut.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Déplacer vers le dossier éléments supprimés via l' [opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent pour l’élément. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour l’élément. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour l’élément. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier éléments supprimés.  <br/> |DeletedEvent à partir du dossier de recherche AllItems par défaut.  <br/> CreatedEvent pour l’élément dans le dossier AllItems.  <br/> ModifiedEvent pour le dossier parent d’origine de l’élément.  <br/> ModifiedEvent pour le dossier éléments supprimés.  <br/> |
|Suppression douce via l' [opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |
|Suppression définitive via l' [opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |
|Déplacer vers le dossier éléments supprimés via l' [opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent pour le dossier. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour le dossier. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour le dossier. Cette énumération spécifie les anciens et les nouveaux identificateurs de dossiers parents.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier éléments supprimés.  <br/> |ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier éléments supprimés.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

