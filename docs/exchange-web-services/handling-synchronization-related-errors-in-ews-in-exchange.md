---
title: Gestion des erreurs liées à la synchronisation dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 6de27d585e467d900941f34b2210877d17205502
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754778"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la synchronisation dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la synchronisation dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Si votre application synchronise les éléments et les dossiers, vous devrez peut-être gérer les erreurs liées à la synchronisation. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS. La plupart de ces erreurs est définie par l’énumération [ResponseCodeType](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) dans l’API managée EWS et l’élément [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) dans Exchange Web Services (EWS). 
  
**Le tableau 1. Erreurs liées à la synchronisation et comment les gérer**

|**Erreur**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | Synchroniser des éléments ou des dossiers à l’aide d’une valeur d’état de synchronisation non valide.  <br/>  Exclure un dossier racine dans votre demande SyncFolderHierarchy initiale, lorsque votre demande ultérieure n’inclut pas un dossier racine.  <br/>  Utiliser les dossiers racine différent dans les demandes suivantes.  <br/> | S’assurer que la valeur d’état de synchronisation à que vous envoyez correspond la valeur d’état de synchronisation renvoyés au cours d’une synchronisation précédente.  <br/>  En vous assurant que vous n’envoyez pas l’état de synchronisation de la hiérarchie de dossiers lorsque vous essayez de synchroniser les éléments et vice versa.  <br/>  En vous assurant que vous envoyez l’état de synchronisation pour le dossier racine correct.  <br/>  S’assurer que le même dossier racine est spécifié dans chaque demande.  <br/>  S’assurer que la demande précédente n’avez pas spécifié un dossier racine de la valeur null, tandis que la demande en cours comporte un dossier racine de la racine. NULL et racine ne sont pas traitées de la même.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Synchroniser les sous-dossiers ou les éléments d’un dossier est introuvable sur le serveur.  <br/> |L’ID spécifié dans la demande en vous assurant que le dossier correspond à un ID de dossier renvoyé à partir du serveur dans une réponse de synchronisation précédente.  <br/> |
|ErrorTimeoutExpired  <br/> |Envoyer un trop grand nombre de demandes.  <br/> |Limiter vos lots à 10 éléments par lot pour éviter les [limitées](ews-throttling-in-exchange.md).  <br/> |
|[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |Se connecter à EWS lorsque le serveur est en mode hors connexion ou il existe un problème de connectivité.  <br/> |Vérification de la connectivité avec le serveur et réessayez votre demande ultérieurement. Il s’agit probablement d’une erreur de service temporaires ou réseau.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Synchroniser les dossiers à l’aide de EWS dans Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Synchroniser des éléments à l’aide de EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

