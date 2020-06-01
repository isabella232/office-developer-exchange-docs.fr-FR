---
title: Gestion des erreurs liées à la délégation dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Découvrez comment gérer les erreurs liées à la délégation dans les applications que vous développez à l’aide de l’API managée EWS ou de EWS dans Exchange.
ms.openlocfilehash: 145783c4e7f49ed6e2aa3a2dbe0d10909e06d7e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455351"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Gestion des erreurs liées à la délégation dans EWS dans Exchange

Découvrez comment gérer les erreurs liées à la délégation dans les applications que vous développez à l’aide de l’API managée EWS ou de EWS dans Exchange.
  
Si votre application utilise la délégation ou ajoute ou supprime des délégués, il se peut que vous deviez gérer les erreurs liées à la délégation. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS. Ces erreurs sont définies par l’API managée EWS [ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) , énumération et par l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) EWS. 
  
## <a name="delegation-related-errors"></a>Erreurs liées à la délégation

|**Error**|**Cet événement se produit lorsque vous essayez de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Effectuer une opération sur une boîte aux lettres, un dossier ou un élément auquel vous n’avez pas accès.  <br/> |Mise à jour des autorisations du délégué afin de les autoriser à accéder au dossier ou à l’élément en appelant la méthode de l’API managée EWS [UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) ou l’opération EWS [UpdateDelegate](https://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) , puis en renouvelant la demande.  <br/> |
|ErrorAccessDenied  <br/> |Modifiez un élément dont vous ne disposez pas de privilèges suffisants pour le modifier.  <br/> |Mise à jour de vos autorisations de délégué en appelant la méthode de l’API managée EWS **UpdateDelegate** ou l’opération EWS **UpdateDelegate** , puis en réessayant la demande.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Tentative d’ajout du propriétaire de la boîte aux lettres en tant que délégué à sa propre boîte aux lettres.  <br/> |[Ajout d’un autre utilisateur en tant que délégué](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md), et non du propriétaire de la boîte aux lettres.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Ajoutez le délégué lorsque le délégué existe déjà.  <br/> |Ne rien faire, car le délégué existe déjà pour le propriétaire de la boîte aux lettres. Ou, si vous essayez de modifier les autorisations d’un délégué existant, utilisez la méthode **UpdateDelegates** ou l’opération **UpdateDelegate** .  <br/> |
|ErrorNotDelegate  <br/> |Modifier les autorisations de délégué pour un utilisateur qui ne dispose pas d’autorisations déléguées pour la boîte aux lettres.  <br/> |[Ajout de l’utilisateur en tant que délégué](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) de la boîte aux lettres avant la tentative de mise à jour ou de suppression des autorisations.  <br/> |
|ErrorDelegateNoUser  <br/> |Modifier les autorisations de délégué pour un utilisateur qui n’est pas dans le service de domaine Active Directory (AD DS).  <br/> |Création de l’utilisateur dans AD DS ou correction des informations de délégué dans la demande.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Utilisez un délégué pour vous abonner aux notifications au nom du propriétaire de la boîte aux lettres.  <br/> |Abonnement aux notifications en tant que propriétaire de la boîte aux lettres.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Faites une demande à partir d’un délégué dont la version de serveur est différente de celle du serveur de boîtes aux lettres du principal.  <br/> |Utilisation d’un délégué ou ajout d’un délégué dont la boîte aux lettres a la même version de serveur que le propriétaire de la boîte aux lettres.  <br/> |
|ErrorMissingEmailAddress  <br/> |Faire une demande à l’aide d’un compte délégué qui n’a pas de boîte aux lettres.  <br/> |Ajout d’une boîte aux lettres au compte du délégué.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

