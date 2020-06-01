---
title: Gestion des erreurs liées à la synchronisation dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: f62937ec444d64b0b358581371f1260f565215b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455939"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la synchronisation dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Si votre application synchronise des éléments et des dossiers, il se peut que vous deviez gérer les erreurs liées à la synchronisation. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS. La plupart de ces erreurs sont définies par l’énumération [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) dans l’API managée EWS et l’élément [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) dans les services Web Exchange (EWS). 
  
**Tableau 1. Erreurs liées à la synchronisation et comment les gérer**

|**Error**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Synchroniser des éléments ou des dossiers à l’aide d’une valeur d’état de synchronisation non valide.  <br/>  Excluez un dossier racine dans votre demande Opérationsyncfolderhierarchy initiale, lorsque votre demande ultérieure inclut un dossier racine.  <br/>  Utiliser des dossiers racine différents dans les demandes ultérieures.  <br/> | Assurez-vous que la valeur d’état de synchronisation que vous envoyez correspond à la valeur d’état de synchronisation renvoyée lors d’une synchronisation précédente.  <br/>  Vérifiez que vous n’envoyez pas l’état de synchronisation pour la hiérarchie de dossiers lorsque vous tentez de synchroniser des éléments, et inversement.  <br/>  Vérifiez que vous envoyez l’état de synchronisation pour le dossier racine correct.  <br/>  Vérifier que le même dossier racine est spécifié dans chaque demande.  <br/>  S’assurer que la demande précédente n’a pas spécifié de dossier racine null, tandis que la demande actuelle inclut un dossier racine racine. NULL et root ne sont pas traités de la même façon.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Synchroniser des sous-dossiers ou des éléments dans un dossier qui est introuvable sur le serveur.  <br/> |S’assurer que l’ID de dossier spécifié dans la demande correspond à un ID de dossier renvoyé par le serveur dans une réponse de synchronisation précédente.  <br/> |
|ErrorTimeoutExpired  <br/> |Envoyer trop de requêtes.  <br/> |Limitation de vos lots à 10 éléments par lot pour éviter d’être [limité](ews-throttling-in-exchange.md).  <br/> |
|[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Connectez-vous à EWS lorsque le serveur est hors connexion ou qu’il y a un problème de connectivité.  <br/> |Vérification de la connectivité avec le serveur et nouvelle tentative ultérieure de votre demande. Il s’agit probablement d’une erreur de service ou d’une erreur réseau passagère.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Synchroniser des dossiers à l’aide d’EWS dans Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Synchroniser des éléments à l’aide d’EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

