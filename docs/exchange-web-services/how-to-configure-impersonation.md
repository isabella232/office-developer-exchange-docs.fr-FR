---
title: Configurer l’emprunt d'identité
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Découvrez comment accorder le rôle d’emprunt d’identité à un compte de service à l’aide de l’environnement de ligne de commande Exchange Management Shell.
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754817"
---
# <a name="configure-impersonation"></a>Configurer l’emprunt d'identité

Découvrez comment accorder le rôle d’emprunt d’identité à un compte de service à l’aide de l’environnement de ligne de commande Exchange Management Shell. 
  
L'emprunt d'identité permet à un appelant, tel qu'une application de service, d'emprunter l'identité d'un compte d'utilisateur. L'appelant peut effectuer des opérations en utilisant les autorisations associées au compte représenté plutôt que celles associées à son propre compte.
  
Exchange Online, Exchange Online dans le cadre d'Office 365 et les versions de Microsoft Exchange à partir d'Exchange 2013 utilisent un contrôle d'accès en fonction du rôle (RBAC) pour attribuer des autorisations aux comptes. Votre administrateur de serveur Exchange devra accorder le rôle **ApplicationImpersonation** à chaque compte de service qui empruntera l'identité d'autres utilisateurs à l'aide de la cmdlet [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx). 
  
## <a name="configuring-the-applicationimpersonation-role"></a>Configuration du rôle ApplicationImpersonation

Lorsque vous ou votre administrateur de serveur Exchange attribuez le rôle **ApplicationImpersonation**, utilisez les paramètres de la cmdlet**New-ManagementRoleAssignment** suivants : 
  
-  _Nom_&ndash;  Nom convivial de l'attribution de rôle. Chaque fois que vous attribuez un rôle, une entrée est créée dans la liste des rôles RBAC. Vous pouvez vérifier les attributions de rôle à l’aide du cmdlet[Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx). 
    
-  _Rôle_&ndash;Rôle RBAC à attribuer. Lorsque vous configurez l’emprunt d’identité, vous attribuez le** rôle ApplicationImpersonation**. 
    
-  _Utilisateur_&ndash;Compte de service. 
    
-  _CustomRecipientScope_&ndash;Étendue des utilisateurs dont le compte de service peut emprunter l'identité. Le compte de service pourra uniquement emprunter l’identité d’autres utilisateurs au sein de l’étendue spécifiée. Si aucune étendue n'est spécifiée, le compte de service dispose du rôle **ApplicationImpersonation** pour tous les utilisateurs de l'organisation. Vous pouvez créer des étendues de gestion personnalisées à l'aide de la cmdlet [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx). 
    
Pour pouvoir configurer l’emprunt d’identité, vous devez disposer des éléments suivants :
  
- Informations d’identification d’administration pour le serveur Exchange.
    
- Informations d’identification de l’administrateur de domaine ou autres informations d’identification accordant l’autorisation de créer, et d’attribuer des rôles et des étendues.
    
- Outils de gestion Exchange. Ces outils sont installés sur l’ordinateur à partir duquel vous allez exécuter les commandes.
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>Configuration de l’emprunt d’identité pour tous les utilisateurs d’une organisation

1. Ouvrez l'environnement de ligne de commande Exchange Management Shell. Dans le menu Démarrer, choisissez **Tous les programmes** > **Microsoft Exchange Server 2013**. 
    
2. Exécutez la cmdlet **New-ManagementRoleAssignment** pour ajouter l'autorisation d'emprunt d'identité à l'utilisateur spécifié. L'exemple suivant montre comment configurer l'emprunt d'identité pour permettre à un compte de service d'emprunter l'identité de tous les autres utilisateurs d'une organisation. 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>Configuration de l’emprunt d’identité pour certains utilisateurs ou groupes d’utilisateurs

1. Ouvrez l'environnement de ligne de commande Exchange Management Shell. Dans le menu Démarrer, choisissez **Tous les programmes** > **Microsoft Exchange Server 2013**. 
    
2. Exécutez la cmdlet **New-ManagementScope** pour créer une étendue à laquelle le rôle d'emprunt d'identité peut être attribué. Si une étendue existante est disponible, vous pouvez ignorer cette étape. L'exemple suivant montre comment créer une étendue de gestion pour un groupe spécifique. 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   Le paramètre_RecipientRestrictionFilter_ de la cmdlet **New-ManagementScope** définit les membres de l'étendue. Vous pouvez utiliser les propriétés de**l’identité**de l’objet pour créer le filtre. L'exemple suivant est un filtre qui limite le résultat à un utilisateur unique avec le nom d'utilisateur « John ». 
    
   ```powershell
   Name -eq "john"
   ```

3. Exécutez la cmdlet **New-ManagementRoleAssignment** pour ajouter l'autorisation d'emprunt d'identité des membres de l'étendue spécifiée. L'exemple suivant montre comment configurer un compte de service pour emprunter l'identité de tous les utilisateurs d'une étendue. 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


Une fois les autorisations d'emprunt d'identité octroyées par votre administrateur, vous pouvez utiliser le compte de service pour émettre des appels pour le compte d'autres utilisateurs. Vous pouvez vérifier les attributions de rôles à l'aide de la cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx). 
  
## <a name="see-also"></a>Voir aussi

- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
- [Rôle ApplicationImpersonation](http://technet.microsoft.com/fr-FR/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

