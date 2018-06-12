---
title: Configurer l’emprunt d’identité
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment accorder le rôle d'emprunt d'identité à un compte de service à l'aide de l'environnement de ligne de commande Exchange Management Shell.
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754817"
---
# <a name="configure-impersonation"></a><span data-ttu-id="56d0b-103">Configurer l’emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="56d0b-103">Configure impersonation</span></span>

<span data-ttu-id="56d0b-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment accorder le rôle d'emprunt d'identité à un compte de service à l'aide de l'environnement de ligne de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="56d0b-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="56d0b-p101">L'emprunt d'identité permet à un appelant, tel qu'une application de service, d'emprunter l'identité d'un compte d'utilisateur. L'appelant peut effectuer des opérations en utilisant les autorisations associées au compte représenté plutôt que celles associées à son propre compte.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p101">Impersonation enables a caller, such as a service application, to impersonate a user account. The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="56d0b-p102">Exchange Online, Exchange Online dans le cadre d'Office 365 et les versions de Microsoft Exchange à partir d'Exchange 2013 utilisent un contrôle d'accès en fonction du rôle (RBAC) pour attribuer des autorisations aux comptes. Votre administrateur de serveur Exchange devra accorder le rôle **ApplicationImpersonation** à chaque compte de service qui empruntera l'identité d'autres utilisateurs à l'aide de la cmdlet [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx).</span><span class="sxs-lookup"><span data-stu-id="56d0b-p102">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts. Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="56d0b-109">Configuration du rôle ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="56d0b-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="56d0b-110">Lorsque vous ou votre administrateur de serveur Exchange attribuez le rôle **ApplicationImpersonation**, utilisez les paramètres de la cmdlet **New-ManagementRoleAssignment** suivants :</span><span class="sxs-lookup"><span data-stu-id="56d0b-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="56d0b-111">_Nom_ &ndash; Le nom convivial de l’attribution de rôle.</span><span class="sxs-lookup"><span data-stu-id="56d0b-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="56d0b-112">Chaque fois que vous attribuez un rôle, une entrée est créée dans la liste des rôles RBAC.</span><span class="sxs-lookup"><span data-stu-id="56d0b-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="56d0b-113">Vous pouvez vérifier les attributions de rôles à l'aide de la cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx).</span><span class="sxs-lookup"><span data-stu-id="56d0b-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="56d0b-114">_Rôle_ &ndash; Rôle RBAC à affecter.</span><span class="sxs-lookup"><span data-stu-id="56d0b-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="56d0b-115">Lorsque vous configurez l'emprunt d'identité, vous attribuez le rôle **ApplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="56d0b-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="56d0b-116">_Utilisateur_ &ndash; Le compte de service.</span><span class="sxs-lookup"><span data-stu-id="56d0b-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="56d0b-117">_CustomRecipientScope_ &ndash; L’étendue d’utilisateurs dont le compte de service peut emprunter l’identité.</span><span class="sxs-lookup"><span data-stu-id="56d0b-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="56d0b-118">Le compte de service pourra uniquement emprunter l'identité d'autres utilisateurs au sein de l'étendue spécifiée.</span><span class="sxs-lookup"><span data-stu-id="56d0b-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="56d0b-119">Si aucune étendue n'est spécifiée, le compte de service dispose du rôle **ApplicationImpersonation** pour tous les utilisateurs de l'organisation.</span><span class="sxs-lookup"><span data-stu-id="56d0b-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="56d0b-120">Vous pouvez créer des étendues de gestion personnalisées à l'aide de la cmdlet [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx).</span><span class="sxs-lookup"><span data-stu-id="56d0b-120">You can create custom management scopes by using the [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="56d0b-121">Pour pouvoir configurer l'emprunt d'identité, vous devez disposer des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="56d0b-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="56d0b-122">Informations d'identification d'administration pour le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="56d0b-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="56d0b-123">Informations d'identification de l'administrateur de domaine ou autres informations d'identification accordant l'autorisation de créer, et d'attribuer des rôles et des étendues.</span><span class="sxs-lookup"><span data-stu-id="56d0b-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="56d0b-p106">Outils de gestion Exchange. Ces outils sont installés sur l'ordinateur à partir duquel vous allez exécuter les commandes.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p106">Exchange management tools. These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="56d0b-126">Configuration de l'emprunt d'identité pour tous les utilisateurs d'une organisation</span><span class="sxs-lookup"><span data-stu-id="56d0b-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="56d0b-p107">Ouvrez l'environnement de ligne de commande Exchange Management Shell. Dans le menu Démarrer, choisissez **Tous les programmes** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p107">Open the Exchange Management Shell. From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="56d0b-p108">Exécutez la cmdlet **New-ManagementRoleAssignment** pour ajouter l'autorisation d'emprunt d'identité à l'utilisateur spécifié. L'exemple suivant montre comment configurer l'emprunt d'identité pour permettre à un compte de service d'emprunter l'identité de tous les autres utilisateurs d'une organisation.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p108">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user. The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="56d0b-131">Configuration de l'emprunt d'identité pour certains utilisateurs ou groupes d'utilisateurs</span><span class="sxs-lookup"><span data-stu-id="56d0b-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="56d0b-p109">Ouvrez l'environnement de ligne de commande Exchange Management Shell. Dans le menu Démarrer, choisissez **Tous les programmes** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p109">Open the Exchange Management Shell. From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="56d0b-p110">Exécutez la cmdlet **New-ManagementScope** pour créer une étendue à laquelle le rôle d'emprunt d'identité peut être attribué. Si une étendue existante est disponible, vous pouvez ignorer cette étape. L'exemple suivant montre comment créer une étendue de gestion pour un groupe spécifique.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p110">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned. If an existing scope is available, you can skip this step. The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="56d0b-137">Le paramètre _RecipientRestrictionFilter_ de l’applet de commande **New-ManagementScope** définit les membres de l’étendue.</span><span class="sxs-lookup"><span data-stu-id="56d0b-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="56d0b-138">Vous pouvez utiliser les propriétés de l'objet **Identity** pour créer le filtre.</span><span class="sxs-lookup"><span data-stu-id="56d0b-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="56d0b-139">L'exemple suivant est un filtre qui limite le résultat à un utilisateur unique avec le nom d'utilisateur « John ».</span><span class="sxs-lookup"><span data-stu-id="56d0b-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="56d0b-p112">Exécutez la cmdlet **New-ManagementRoleAssignment** pour ajouter l'autorisation d'emprunt d'identité des membres de l'étendue spécifiée. L'exemple suivant montre comment configurer un compte de service pour emprunter l'identité de tous les utilisateurs d'une étendue.</span><span class="sxs-lookup"><span data-stu-id="56d0b-p112">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope. The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="56d0b-p113">Une fois les autorisations d'emprunt d'identité octroyées par votre administrateur, vous pouvez utiliser le compte de service pour émettre des appels pour le compte d'autres utilisateurs. Vous pouvez vérifier les attributions de rôles à l'aide de la cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx).</span><span class="sxs-lookup"><span data-stu-id="56d0b-p113">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts. You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="56d0b-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="56d0b-144">See also</span></span>

- [<span data-ttu-id="56d0b-145">Emprunt d'identité et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="56d0b-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="56d0b-146">Rôle ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="56d0b-146">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="56d0b-147">New-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="56d0b-147">New-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="56d0b-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="56d0b-148">Get-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    
