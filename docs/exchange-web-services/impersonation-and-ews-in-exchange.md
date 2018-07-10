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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754957"
---
# <a name="impersonation-and-ews-in-exchange"></a><span data-ttu-id="d76af-103">Emprunt d'identité et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d76af-103">Impersonation and EWS in Exchange</span></span>

<span data-ttu-id="d76af-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment et dans quels cas utiliser l'emprunt d'identité dans vos [applications de service](ews-application-types.md) Exchange.</span><span class="sxs-lookup"><span data-stu-id="d76af-104">Learn how and when to use impersonation in your Exchange [service applications](ews-application-types.md).</span></span>
  
<span data-ttu-id="d76af-105">Vous pouvez permettre à des utilisateurs d'accéder aux boîtes aux lettres d'autres utilisateurs de trois façons :</span><span class="sxs-lookup"><span data-stu-id="d76af-105">You can enable users to access other users' mailboxes in one of three ways:</span></span>
  
- <span data-ttu-id="d76af-106">En ajoutant des délégués et en spécifiant des autorisations pour chacun d'entre eux.</span><span class="sxs-lookup"><span data-stu-id="d76af-106">By adding delegates and specifying permissions for each delegate.</span></span>
    
- <span data-ttu-id="d76af-107">En modifiant directement les autorisations du dossier.</span><span class="sxs-lookup"><span data-stu-id="d76af-107">By modifying folder permissions directly.</span></span>
    
- <span data-ttu-id="d76af-108">En utilisant l'emprunt d'identité.</span><span class="sxs-lookup"><span data-stu-id="d76af-108">By using impersonation.</span></span>
    
<span data-ttu-id="d76af-p101">Dans quels cas choisir l'emprunt d'identité plutôt que la délégation ou les autorisations de dossier ? Consultez les conseils ci-dessous pour déterminer la méthode la plus adaptée :</span><span class="sxs-lookup"><span data-stu-id="d76af-p101">When should you choose impersonation over delegation or folder permissions? The following guidelines will help you decide:</span></span>
  
- <span data-ttu-id="d76af-111">Utilisez les autorisations de dossier lorsque vous souhaitez octroyer l'accès à un dossier à un utilisateur, mais que vous ne souhaitez pas que ce dernier dispose des autorisations « Envoyer de la part de ».</span><span class="sxs-lookup"><span data-stu-id="d76af-111">Use folder permissions when you want to provide a user access to a folder but do not want the user to have "send on behalf of" permissions.</span></span> 
    
- <span data-ttu-id="d76af-p102">Utilisez l'accès délégué lorsque vous souhaitez donner à un utilisateur l'autorisation d'effectuer une tâche pour le compte d'un autre utilisateur. En règle générale, il s'agit d'une autorisation concernant une personne ou un nombre restreint d'utilisateurs : par exemple, un assistant administratif qui gère le calendrier d'un administrateur, ou une personne chargée de la planification des salles qui gère les calendriers de plusieurs salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="d76af-p102">Use delegate access when you want to give one user permission to perform work on behalf of another user. Typically, this is a one-to-one or one-to-a-few permission - for example, a single administrative assistant managing the calendar for an administrator, or a single room scheduler managing the calendars for a group of meeting rooms.</span></span>
    
- <span data-ttu-id="d76af-114">Utilisez l'emprunt d'identité lorsque vous disposez d'une application de service qui doit accéder à plusieurs boîtes aux lettres et « agir en tant que » propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d76af-114">Use impersonation when you have a service application that needs to access multiple mailboxes and "act as" the mailbox owner.</span></span>
    
<span data-ttu-id="d76af-p103">L'emprunt d'identité est la solution la plus adaptée lorsque vous utilisez plusieurs boîtes aux lettres, car vous pouvez facilement accorder un accès à un compte de service pour chaque boîte aux lettres dans une base de données. La délégation et les autorisations de dossier conviennent mieux si vous souhaitez accorder l'accès uniquement à certains utilisateurs, car vous devez ajouter les autorisations individuellement pour chaque boîte aux lettres. La Figure 1 présente quelques-unes des différences entre chaque type d'accès.</span><span class="sxs-lookup"><span data-stu-id="d76af-p103">Impersonation is the best choice when you're dealing with multiple mailboxes because you can easily grant one service account access to every mailbox in a database. Delegation and folder permissions are best when you're only granting access to a few users, because you have to add permissions individually to each mailbox. Figure 1 shows some of the differences between each type of access.</span></span>
  
<span data-ttu-id="d76af-118">**Figure 1. Méthodes d'accès aux boîtes aux lettres des autres utilisateurs**</span><span class="sxs-lookup"><span data-stu-id="d76af-118">**Figure 1. Ways to access other users' mailboxes**</span></span>

![Diagramme montrant les types d'accès à la boîte aux lettres, la relation entre les propriétaires de boîtes aux lettres et le délégué pour chaque type, ainsi que le type d'autorisation. Autorisations « Envoyer pour le compte de » pour les autorisations de dossier et/ou délégation. Autorisations « Envoyer en tant que » pour l'emprunt d'identité.](media/Ex15_Delegate_Overview.png)
  
<span data-ttu-id="d76af-p105">L'emprunt d'identité est idéal pour les applications qui se connectent à Exchange Online, Exchange Online dans le cadre d'Office 365 et aux versions locales d'Exchange, et qui effectuent des opérations, telles que l'archivage des messages électroniques, la configuration automatique des messages d'absence pour les utilisateurs en congés ou toute autre tâche qui nécessite que l'application agisse en tant que propriétaire d'une boîte aux lettres. Lorsqu'une application utilise l'emprunt d'identité pour envoyer un message, l'e-mail apparaît comme envoyé par le propriétaire de la boîte aux lettres. Il n'existe aucun moyen pour le destinataire de savoir que le message a été envoyé par le compte de service. À l'inverse, la délégation permet d'octroyer à un autre compte de boîte aux lettres l'autorisation d'agir au nom du propriétaire de la boîte aux lettres. Lorsqu'un e-mail est envoyé par un délégué, la valeur « De » identifie le propriétaire de la boîte aux lettres, tandis que la valeur « Expéditeur » identifie le délégué qui a envoyé le message.</span><span class="sxs-lookup"><span data-stu-id="d76af-p105">Impersonation is ideal for applications that connect to Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange and perform operations, such as archiving email, setting OOF automatically for users on vacation, or any other task that requires that the application act as the owner of a mailbox. When an application uses impersonation to send a message, the email appears to be sent from the mailbox owner. There is no way for the recipient to know the mail was sent by the service account. Delegation, on the other hand, gives another mailbox account permission to act on behalf of a mailbox owner. When an email message is sent by a delegate, the "from" value identifies the mailbox owner, and the "sender" value identifies the delegate that sent the mail.</span></span> 
  
## <a name="security-considerations-for-impersonation"></a><span data-ttu-id="d76af-127">Considérations relatives à la sécurité dans le cadre de l'emprunt d'identité</span><span class="sxs-lookup"><span data-stu-id="d76af-127">Security considerations for impersonation</span></span>

<span data-ttu-id="d76af-p106">L'emprunt d'identité permet à un appelant d'emprunter l'identité d'un compte d'utilisateur donné. Cela permet à l'appelant d'effectuer des opérations en utilisant les autorisations associées au compte représenté, plutôt que celles associées à son propre compte. Pour cette raison, vous devez prendre en considération les points relatifs à la sécurité ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="d76af-p106">Impersonation enables a caller to impersonate a given user account. This enables the caller to perform operations by using the permissions that are associated with the impersonated account, instead of the permissions that are associated with the caller's account. For this reason, you should be aware of the following security considerations:</span></span>
  
- <span data-ttu-id="d76af-131">Seuls les comptes auxquels le rôle **ApplicationImpersonation** a été attribué par un administrateur de serveur Exchange peuvent utiliser l'emprunt d'identité.</span><span class="sxs-lookup"><span data-stu-id="d76af-131">Only accounts that have been granted the **ApplicationImpersonation** role by an Exchange server administrator can use impersonation.</span></span> 
    
- <span data-ttu-id="d76af-p107">Vous devez créer une étendue de gestion qui limite l'emprunt d'identité à un groupe de comptes spécifié. Si vous ne créez pas d'étendue de gestion, le rôle **ApplicationImpersonation** est attribué à tous les comptes de l'organisation.</span><span class="sxs-lookup"><span data-stu-id="d76af-p107">You should create a management scope that limits impersonation to a specified group of accounts. If you do not create a management scope, the **ApplicationImpersonation** role is granted to all accounts in an organization.</span></span> 
    
- <span data-ttu-id="d76af-p108">En règle générale, le rôle **ApplicationImpersonation** est attribué à un compte de service dédié à une application ou un groupe d'applications spécifique, plutôt qu'à un compte d'utilisateur. Vous pouvez créer autant de comptes de service que nécessaire.</span><span class="sxs-lookup"><span data-stu-id="d76af-p108">Typically, the **ApplicationImpersonation** role is granted to a service account dedicated to a particular application or group of applications, rather than a user account. You can create as many or as few service accounts as you need.</span></span> 
    
<span data-ttu-id="d76af-136">Vous pouvez trouver davantage d'informations sur la [configuration d'emprunt d'identité](how-to-configure-impersonation.md), mais vous devez vous assurer auprès de votre administrateur Exchange que les comptes de service dont vous avez besoin sont créés avec des [accès et des autorisations](http://technet.microsoft.com/fr-fr/library/dd351175%28v=exchg.150%29.aspx) respectant les exigences de sécurité de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="d76af-136">You can read more about [configuring impersonation](how-to-configure-impersonation.md), but you should work with your Exchange administrator to ensure that the service accounts that you need are created with the [permissions and access](http://technet.microsoft.com/fr-fr/library/dd351175%28v=exchg.150%29.aspx) that meet the security requirements of your organization.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="d76af-137">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="d76af-137">In this section</span></span>

- [<span data-ttu-id="d76af-138">Configurer l’emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="d76af-138">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="d76af-139">Identifier le compte pour emprunter l’identité</span><span class="sxs-lookup"><span data-stu-id="d76af-139">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="d76af-140">Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange</span><span class="sxs-lookup"><span data-stu-id="d76af-140">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a><span data-ttu-id="d76af-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d76af-141">See also</span></span>


- [<span data-ttu-id="d76af-142">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d76af-142">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="d76af-143">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d76af-143">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d76af-144">Autorisations Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d76af-144">Exchange 2013 Permissions</span></span>](http://technet.microsoft.com/fr-fr/library/dd351175%28v=exchg.150%29.aspx)
    

