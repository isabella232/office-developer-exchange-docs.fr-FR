---
title: Gestion des erreurs liées à la synchronisation dans EWS Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API manaie EWS ou d’EWS dans Exchange.
ms.openlocfilehash: fd52b54413c6fc791132fb01b47bc9077d0266b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513247"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la synchronisation dans EWS Exchange

Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API manaie EWS ou d’EWS dans Exchange.
  
Si votre application synchronise des éléments et des dossiers, vous de devez peut-être gérer les erreurs liées à la synchronisation. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS. La plupart de ces erreurs sont définies par l’éumération [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) dans l’API gérée EWS et par l’élément [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) dans Exchange Web Services (EWS). 
  
**Tableau 1. Erreurs liées à la synchronisation et comment les gérer**

|**Erreur**|**Se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Synchroniser des éléments ou des dossiers à l’aide d’une valeur d’état de synchronisation non valide.  <br/>  Excluez un dossier racine dans votre demande SyncFolderHierarchy initiale, lorsque votre requête suivante inclut un dossier racine.  <br/>  Utilisez différents dossiers racine dans les demandes suivantes.  <br/> | S’assurer que la valeur d’état de synchronisation que vous envoyez correspond à la valeur de l’état de synchronisation renvoyée lors d’une synchronisation précédente.  <br/>  S’assurer que vous n’envoyez pas l’état de synchronisation pour la hiérarchie de dossiers lorsque vous essayez de synchroniser des éléments, et inversement.  <br/>  S’assurer que vous envoyez l’état de synchronisation pour le dossier racine correct.  <br/>  S’assurer que le même dossier racine est spécifié dans chaque demande.  <br/>  S’assurer que la demande précédente n’a pas spécifié de dossier racine null, tandis que la demande actuelle inclut un dossier racine de la racine. Null et root ne sont pas traités de la même manière.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Synchroniser les sous-dossiers ou les éléments d’un dossier qui ne sont pas trouvés sur le serveur.  <br/> |S’assurer que l’ID de dossier spécifié dans la demande correspond à un ID de dossier renvoyé par le serveur dans une réponse de synchronisation précédente.  <br/> |
|ErrorTimeoutExpired  <br/> |Envoyer trop de demandes.  <br/> |Limiter vos lots à 10 éléments par lot pour éviter [d’être limité.](ews-throttling-in-exchange.md)  <br/> |
|[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Connecter EWS lorsque le serveur est hors connexion ou qu’il y a un problème de connectivité.  <br/> |Vérification de la connectivité avec le serveur et nouvelle tentative de votre demande ultérieurement. Il s’agit probablement d’une erreur de service temporaire ou d’une erreur réseau.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Synchroniser des dossiers à l’aide d’EWS Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Synchroniser des éléments à l’aide d’EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

