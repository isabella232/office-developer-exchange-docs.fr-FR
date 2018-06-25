---
title: Gestion des erreurs liées à la délégation dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Découvrez comment gérer les erreurs liées à la délégation dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 3851709888e3a1087df02eea5d4d58888ad168e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754774"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la délégation dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la délégation dans les applications que vous développez à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Si votre application utilise la délégation ou ajoute ou supprime des délégués, vous devrez peut-être gérer les erreurs liées à la délégation. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS. Ces erreurs sont définies par l’énumération API managées [constatez](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) et l’élément EWS [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) . 
  
## <a name="delegation-related-errors"></a>Erreurs liées à la délégation

|**Erreur**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Effectuer une opération sur une boîte aux lettres, un dossier ou un élément que vous n’avez pas accès à.  <br/> |Mise à jour les autorisations du délégué pour leur permettre d’accès du dossier ou un élément en appelant la méthode d’API managées [UpdateDelegates](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) ou l’opération EWS [UpdateDelegate](http://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) , puis une nouvelle tentative de la demande.  <br/> |
|ErrorAccessDenied  <br/> |Modifier un élément que vous n’avez pas de privilèges suffisants pour modifier.  <br/> |Mise à jour votre déléguer des autorisations en appelant la méthode d’API managées **UpdateDelegate** ou l’opération EWS **UpdateDelegate** , puis une nouvelle tentative de la demande.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Essayez d’ajouter le propriétaire de la boîte aux lettres en tant que délégué à leur propre boîte aux lettres.  <br/> |[Ajout d’un autre utilisateur en tant que délégué](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md), pas le propriétaire de boîte aux lettres.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Ajoutez le délégué lorsque le délégué existe déjà.  <br/> |Faites rien, car le délégué existe déjà pour le propriétaire de boîte aux lettres. Ou, si vous essayez de modifier les autorisations d’un délégué existant, puis utilisez la méthode **UpdateDelegates** ou l’opération **UpdateDelegate** .  <br/> |
|ErrorNotDelegate  <br/> |Modifier les autorisations de délégué pour un utilisateur ayant pas déléguer des autorisations pour la boîte aux lettres.  <br/> |[Ajout de l’utilisateur en tant que délégué](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) pour la boîte aux lettres avant d’essayer de mettre à jour ou de supprimer leurs autorisations.  <br/> |
|ErrorDelegateNoUser  <br/> |Modifier les autorisations de délégué pour un utilisateur qui ne figure pas dans les services de domaine Active Directory (AD DS).  <br/> |Création de l’utilisateur dans AD DS, ou pour corriger les informations du délégué dans la demande.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Utilisez un délégué pour vous abonner aux notifications part le propriétaire de la boîte aux lettres.  <br/> |Abonnement aux notifications en tant que propriétaire de la boîte aux lettres.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Effectuer une demande d’un délégué qui a une version serveur autre que le serveur de boîtes aux lettres de l’entité de sécurité.  <br/> |À l’aide d’un délégué ou en ajoutant un délégué de boîte aux lettres a la même version du serveur en tant que propriétaire de la boîte aux lettres.  <br/> |
|ErrorMissingEmailAddress  <br/> |Effectuer une demande à l’aide d’un compte délégué qui ne dispose pas d’une boîte aux lettres.  <br/> |Ajout d’une boîte aux lettres au compte du délégué.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

