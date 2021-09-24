---
title: Notifications de pull pour les événements de boîte aux lettres liés à la suppression d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Découvrez les événements de boîte aux lettres qui sont produits lorsque vous supprimez des éléments à l’aide d’EWS Exchange.
ms.openlocfilehash: fa04d49f02cfec621f00a9b51b121cff22ca393b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510413"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Notifications de pull pour les événements de boîte aux lettres liés à la suppression d’EWS dans Exchange

Découvrez les événements de boîte aux lettres qui sont produits lorsque vous supprimez des éléments à l’aide d’EWS Exchange.
  
Lorsque vous [supprimez des éléments et des dossiers d’une](deleting-items-by-using-ews-in-exchange.md)boîte aux lettres, cela déclenche un événement de boîte aux lettres. Différentes versions de Exchange événements de boîte aux lettres en réponse aux modifications apportées aux éléments et dossiers d’une boîte aux lettres. Le tableau suivant identifie les événements de boîte aux lettres renvoyés pour les suppressions lorsque vous utilisez des notifications de pull pour vous abonner à des événements de boîte aux lettres. 
  
**Tableau 1 : Événements de boîte aux lettres liés à la suppression pour les notifications de pull**

|**Type de suppression et opération EWS**|**Exchange 2010 lorsque vous spécifiez chaque identificateur de dossier**|**Exchange 2010 lorsque vous spécifiez tous les dossiers**|**Exchange Online notification Exchange 2013 lorsque vous spécifiez chaque identificateur de dossier**|**Exchange Online et Exchange 2013 lorsque vous spécifiez tous les dossiers**|
|:-----|:-----|:-----|:-----|:-----|
|Suppression à l’aide de [l’opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |MovedEvent pour l’élément. Cela spécifie l’ancien et le nouvel identificateur de dossier parent. L’élément est déplacé vers le dossier Suppressions dans la benne.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément du dossier de recherche par défaut AllItems.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Suppression en dur via [l’opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément du dossier de recherche par défaut AllItems.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Déplacer vers le dossier Éléments supprimés via [l’opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent pour l’élément. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier Éléments supprimés.  <br/> |MovedEvent pour l’élément. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier Éléments supprimés.  <br/> |MovedEvent pour l’élément. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent de l’élément.  <br/> ModifiedEvent pour le nouveau dossier parent de l’élément, qui est le dossier Éléments supprimés.  <br/> |DeletedEvent du dossier de recherche par défaut AllItems.  <br/> CreatedEvent pour l’élément dans le dossier AllItems.  <br/> ModifiedEvent pour le dossier parent d’origine de l’élément.  <br/> ModifiedEvent pour le dossier Éléments supprimés.  <br/> |
|Suppression à l’aide de [l’opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |
|Suppression en dur via [l’opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent du dossier.  <br/> |
|Déplacer vers le dossier Éléments supprimés via [l’opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent pour le dossier. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier Éléments supprimés.  <br/> |MovedEvent pour le dossier. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier Éléments supprimés.  <br/> |MovedEvent pour le dossier. Cela spécifie l’ancien et le nouvel identificateur de dossier parent.  <br/> ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier Éléments supprimés.  <br/> |ModifiedEvent pour l’ancien dossier parent du dossier.  <br/> ModifiedEvent pour le nouveau dossier parent du dossier, qui est le dossier Éléments supprimés.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées à la suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

