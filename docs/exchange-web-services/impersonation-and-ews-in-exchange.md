---
title: Emprunt d'identité et EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Découvrez comment et dans quels cas utiliser l'emprunt d'identité dans vos applications de service Exchange.
ms.openlocfilehash: f8a215874475034f0d147b80a05cae414e6438f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754957"
---
# <a name="impersonation-and-ews-in-exchange"></a>Emprunt d'identité et EWS dans Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment et dans quels cas utiliser l'emprunt d'identité dans vos [applications de service](ews-application-types.md) Exchange.
  
Vous pouvez permettre à des utilisateurs d'accéder aux boîtes aux lettres d'autres utilisateurs de trois façons :
  
- En ajoutant des délégués et en spécifiant des autorisations pour chacun d'entre eux.
    
- En modifiant directement les autorisations du dossier.
    
- En utilisant l'emprunt d'identité.
    
Dans quels cas choisir l'emprunt d'identité plutôt que la délégation ou les autorisations de dossier ? Consultez les conseils ci-dessous pour déterminer la méthode la plus adaptée :
  
- Utilisez les autorisations de dossier lorsque vous souhaitez octroyer l'accès à un dossier à un utilisateur, mais que vous ne souhaitez pas que ce dernier dispose des autorisations « Envoyer de la part de ». 
    
- Utilisez l'accès délégué lorsque vous souhaitez donner à un utilisateur l'autorisation d'effectuer une tâche pour le compte d'un autre utilisateur. En règle générale, il s'agit d'une autorisation concernant une personne ou un nombre restreint d'utilisateurs : par exemple, un assistant administratif qui gère le calendrier d'un administrateur, ou une personne chargée de la planification des salles qui gère les calendriers de plusieurs salles de réunion.
    
- Utilisez l'emprunt d'identité lorsque vous disposez d'une application de service qui doit accéder à plusieurs boîtes aux lettres et « agir en tant que » propriétaire de la boîte aux lettres.
    
L'emprunt d'identité est la solution la plus adaptée lorsque vous utilisez plusieurs boîtes aux lettres, car vous pouvez facilement accorder un accès à un compte de service pour chaque boîte aux lettres dans une base de données. La délégation et les autorisations de dossier conviennent mieux si vous souhaitez accorder l'accès uniquement à certains utilisateurs, car vous devez ajouter les autorisations individuellement pour chaque boîte aux lettres. La Figure 1 présente quelques-unes des différences entre chaque type d'accès.
  
**Figure 1. Méthodes d'accès aux boîtes aux lettres des autres utilisateurs**

![Diagramme montrant les types d'accès à la boîte aux lettres, la relation entre les propriétaires de boîtes aux lettres et le délégué pour chaque type, ainsi que le type d'autorisation. Autorisations « Envoyer pour le compte de » pour les autorisations de dossier et/ou délégation. Autorisations « Envoyer en tant que » pour l'emprunt d'identité.](media/Ex15_Delegate_Overview.png)
  
L'emprunt d'identité est idéal pour les applications qui se connectent à Exchange Online, Exchange Online dans le cadre d'Office 365 et aux versions locales d'Exchange, et qui effectuent des opérations, telles que l'archivage des messages électroniques, la configuration automatique des messages d'absence pour les utilisateurs en congés ou toute autre tâche qui nécessite que l'application agisse en tant que propriétaire d'une boîte aux lettres. Lorsqu'une application utilise l'emprunt d'identité pour envoyer un message, l'e-mail apparaît comme envoyé par le propriétaire de la boîte aux lettres. Il n'existe aucun moyen pour le destinataire de savoir que le message a été envoyé par le compte de service. À l'inverse, la délégation permet d'octroyer à un autre compte de boîte aux lettres l'autorisation d'agir au nom du propriétaire de la boîte aux lettres. Lorsqu'un e-mail est envoyé par un délégué, la valeur « De » identifie le propriétaire de la boîte aux lettres, tandis que la valeur « Expéditeur » identifie le délégué qui a envoyé le message. 
  
## <a name="security-considerations-for-impersonation"></a>Considérations relatives à la sécurité dans le cadre de l'emprunt d'identité

L'emprunt d'identité permet à un appelant d'emprunter l'identité d'un compte d'utilisateur donné. Cela permet à l'appelant d'effectuer des opérations en utilisant les autorisations associées au compte représenté, plutôt que celles associées à son propre compte. Pour cette raison, vous devez prendre en considération les points relatifs à la sécurité ci-dessous :
  
- Seuls les comptes auxquels le rôle **ApplicationImpersonation** a été attribué par un administrateur de serveur Exchange peuvent utiliser l'emprunt d'identité. 
    
- Vous devez créer une étendue de gestion qui limite l'emprunt d'identité à un groupe de comptes spécifié. Si vous ne créez pas d'étendue de gestion, le rôle **ApplicationImpersonation** est attribué à tous les comptes de l'organisation. 
    
- En règle générale, le rôle **ApplicationImpersonation** est attribué à un compte de service dédié à une application ou un groupe d'applications spécifique, plutôt qu'à un compte d'utilisateur. Vous pouvez créer autant de comptes de service que nécessaire. 
    
Vous pouvez trouver davantage d'informations sur la [configuration d'emprunt d'identité](how-to-configure-impersonation.md), mais vous devez vous assurer auprès de votre administrateur Exchange que les comptes de service dont vous avez besoin sont créés avec des [accès et des autorisations](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx) respectant les exigences de sécurité de votre organisation. 
  
## <a name="in-this-section"></a>Dans cette section

- [Configurer l’emprunt d’identité](how-to-configure-impersonation.md)
    
- [Identifier le compte pour emprunter l’identité](how-to-identify-the-account-to-impersonate.md)
    
- [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Autorisations Exchange 2013](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx)
    

