---
title: Extraction des notifications pour les événements liés à la suppression de boîte aux lettres EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Découvrir les boîtes aux lettres sont déclenchés lorsque vous supprimez des éléments à l’aide de EWS dans Exchange.
ms.openlocfilehash: b12d6a16cc539f36b6b4dcd7274529e9def3c247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755064"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Extraction des notifications pour les événements liés à la suppression de boîte aux lettres EWS dans Exchange

Découvrir les boîtes aux lettres sont déclenchés lorsque vous supprimez des éléments à l’aide de EWS dans Exchange.
  
Lorsque vous [supprimez les éléments et dossiers à partir d’une boîte aux lettres](deleting-items-by-using-ews-in-exchange.md), cela déclenche un événement de boîte aux lettres. Différentes versions d’Exchange renvoient des événements de boîte aux lettres différente en réponse aux modifications apportées à des éléments et des dossiers dans une boîte aux lettres. Le tableau suivant identifie les événements de boîte aux lettres qui sont renvoyés pour les suppressions lorsque vous utilisez des notifications de type pull s’abonner à des événements de boîte aux lettres. 
  
**Tableau 1 : Les événements liés à la suppression de boîte aux lettres pour les notifications de type pull**

|**Type de suppression et de l’opération EWS**|**Notification d’Exchange 2010 lorsque vous spécifiez l’identificateur de chaque dossier**|**Notification d’Exchange 2010 lorsque vous spécifiez tous les dossiers**|**Exchange Online et Exchange 2013 notification lorsque vous spécifiez l’identificateur de chaque dossier**|**Exchange Online et Exchange 2013 lorsque vous spécifiez tous les dossiers**|
|:-----|:-----|:-----|:-----|:-----|
|Suppression réversible par le biais de l' [opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |MovedEvent pour l’élément. Spécifie les deux les identificateurs de dossier ancien et le nouveau parent. L’élément est déplacé vers le dossier suppressions dans la benne.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément à partir du dossier de recherche par défaut AllItems.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Suppression définitive par le biais de l' [opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |DeletedEvent pour l’élément.  <br/> DeletedEvent pour l’élément à partir du dossier de recherche par défaut AllItems.  <br/> ModifiedEvent pour le dossier parent de l’élément.  <br/> |
|Déplacer vers le dossier éléments supprimés par le biais de l' [opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent pour l’élément. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour le dossier parent ancien de l’élément.  <br/> ModifiedEvent pour nouveau dossier parent l’élément, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour l’élément. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour le dossier parent ancien de l’élément.  <br/> ModifiedEvent pour nouveau dossier parent l’élément, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour l’élément. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour le dossier parent ancien de l’élément.  <br/> ModifiedEvent pour nouveau dossier parent l’élément, qui est le dossier éléments supprimés.  <br/> |DeletedEvent à partir du dossier de recherche par défaut AllItems.  <br/> CreatedEvent pour un élément dans le dossier AllItems.  <br/> ModifiedEvent pour le dossier parent d’origine de l’élément.  <br/> ModifiedEvent pour le dossier éléments supprimés.  <br/> |
|Suppression réversible par le biais de l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |
|Suppression définitive par le biais de l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |DeletedEvent pour le dossier.  <br/> ModifiedEvent pour le dossier parent.  <br/> |
|Déplacer vers le dossier éléments supprimés par le biais de l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent pour le dossier. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour l’ancien dossier parent.  <br/> ModifiedEvent pour le nouveau dossier parent, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour le dossier. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour l’ancien dossier parent.  <br/> ModifiedEvent pour le nouveau dossier parent, qui est le dossier éléments supprimés.  <br/> |MovedEvent pour le dossier. Spécifie les identificateurs de dossier ancien et le nouveau parent.  <br/> ModifiedEvent pour l’ancien dossier parent.  <br/> ModifiedEvent pour le nouveau dossier parent, qui est le dossier éléments supprimés.  <br/> |ModifiedEvent pour l’ancien dossier parent.  <br/> ModifiedEvent pour le nouveau dossier parent qui est le dossier éléments supprimés.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Gestion des erreurs liées aux suppression dans EWS dans Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

