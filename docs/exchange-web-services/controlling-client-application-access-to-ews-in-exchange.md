---
title: Contrôle de l’accès aux applications de client pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Découvrez les options de gestion des accès aux applications de client à EWS.
ms.openlocfilehash: 29a640178afc9814a0b2232225ae4307e49afed2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754764"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="ec02f-103">Contrôle de l’accès aux applications de client pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec02f-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="ec02f-104">Découvrez les options de gestion des accès aux applications de client à EWS.</span><span class="sxs-lookup"><span data-stu-id="ec02f-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="ec02f-105">N’importe quelle application client EWS que vous créez doit avoir accès à Exchange Online, Exchange Online dans le cadre d’Office 365, ou une version d’Exchange, commençant par Exchange 2013 avant de pouvoir appeler des opérations EWS.</span><span class="sxs-lookup"><span data-stu-id="ec02f-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="ec02f-106">Administrateurs de serveur de test ou de production peuvent utiliser Exchange Management Shell pour limiter l’accès à EWS pour tous les utilisateurs et des applications, pour des utilisateurs individuels ou pour des applications individuelles.</span><span class="sxs-lookup"><span data-stu-id="ec02f-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="ec02f-107">Contrôle d’accès pour EWS est basé sur les comptes de domaine.</span><span class="sxs-lookup"><span data-stu-id="ec02f-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="ec02f-108">Lorsqu’une connexion est établie avec les informations d’identification qui sont authentifiées par l’autorité de sécurité locale, le serveur renvoie une erreur indiquant que seuls les comptes de domaine peuvent se connecter.</span><span class="sxs-lookup"><span data-stu-id="ec02f-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="ec02f-109">Contrôle d’accès pour les utilisateurs et les clients EWS</span><span class="sxs-lookup"><span data-stu-id="ec02f-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="ec02f-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="ec02f-110"></span></span>

<span data-ttu-id="ec02f-111">Votre administrateur de serveur de test ou de production permettre configurer le contrôle d’accès pour les clients qui se connectent à EWS comme suit :</span><span class="sxs-lookup"><span data-stu-id="ec02f-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="ec02f-112">En bloquant toutes les applications clientes de se connecter.</span><span class="sxs-lookup"><span data-stu-id="ec02f-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="ec02f-113">Par ainsi que pour la connexion client spécifique.</span><span class="sxs-lookup"><span data-stu-id="ec02f-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="ec02f-114">En autorisant n’importe quelle application client à se connecter à l’exception de ceux qui sont spécifiquement bloqués.</span><span class="sxs-lookup"><span data-stu-id="ec02f-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="ec02f-115">En autorisant n’importe quelle application client à se connecter.</span><span class="sxs-lookup"><span data-stu-id="ec02f-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="ec02f-116">Les applications sont identifiées par la chaîne d’agent utilisateur qu’ils envoient dans la requête web HTTP.</span><span class="sxs-lookup"><span data-stu-id="ec02f-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [! Remarque sur la sécurité]<span data-ttu-id="ec02f-117"> niveau Application blocage n’est pas une fonctionnalité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="ec02f-117"> Application-level blocking is not a security feature.</span></span> <span data-ttu-id="ec02f-118">La chaîne d’agent utilisateur est facilement usurpée.</span><span class="sxs-lookup"><span data-stu-id="ec02f-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="ec02f-119">Si une application est autorisée à accéder à EWS, l’application doit toujours présenter des informations d’identification que le serveur authentifie avant de l’application peut se connecter à EWS.</span><span class="sxs-lookup"><span data-stu-id="ec02f-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="ec02f-120">Les administrateurs peuvent configurer également le contrôle d’accès pour les propriétaires de boîte aux lettres qui se connectent à EWS comme suit :</span><span class="sxs-lookup"><span data-stu-id="ec02f-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="ec02f-121">Bloquer ou autoriser un ensemble de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="ec02f-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="ec02f-122">Bloquer ou autoriser un groupe d’utilisateurs identifié par une étendue de l’authentification basée sur les rôles qui inclut ou exclut les propriétaires de boîte aux lettres qui n’ont pas accès à EWS.</span><span class="sxs-lookup"><span data-stu-id="ec02f-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="ec02f-123">Bloquer ou autoriser un propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ec02f-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="ec02f-124">Paramètres de contrôle d’accès spécifiques remplacent les paramètres de contrôle d’accès général.</span><span class="sxs-lookup"><span data-stu-id="ec02f-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="ec02f-125">Par exemple, si une organisation refuse l’accès EWS, mais un propriétaire de boîte aux lettres est autorisé l’accès de l’application, le paramètre prévaut et l’accès est autorisé.</span><span class="sxs-lookup"><span data-stu-id="ec02f-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="ec02f-126">Délégation et gestion des accès EWS</span><span class="sxs-lookup"><span data-stu-id="ec02f-126">Delegation and EWS access management</span></span>
<span data-ttu-id="ec02f-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="ec02f-127"></span></span>

<span data-ttu-id="ec02f-128">Lorsque les utilisateurs délégués qui n’ont pas accès à EWS utiliser votre application cliente, ils ne pourront accéder aux boîtes aux lettres de l’utilisateur principal à l’aide de EWS, même si l’utilisateur principal a EWS accéder.</span><span class="sxs-lookup"><span data-stu-id="ec02f-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="ec02f-129">Si l’utilisateur délégué dispose d’un accès EWS, le délégué sera en mesure d’utiliser votre application de client EWS pour accéder aux boîtes aux lettres de l’utilisateur principal, même si l’utilisateur principal n’a pas EWS access.</span><span class="sxs-lookup"><span data-stu-id="ec02f-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="ec02f-130">Emprunt d’identité et de gestion de l’accès EWS</span><span class="sxs-lookup"><span data-stu-id="ec02f-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="ec02f-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="ec02f-131"></span></span>

<span data-ttu-id="ec02f-132">Applications clientes qui se connectent à EWS part propriétaires de boîte aux lettres ne peuvent pas être en mesure d’utiliser les paramètres EWS du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ec02f-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="ec02f-133">Par exemple, une application qui archive les e-mails les messages pour une société a pour se connecter à EWS indépendamment des paramètres de rôle la boîte aux lettres des utilisateurs sont.</span><span class="sxs-lookup"><span data-stu-id="ec02f-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="ec02f-134">Autres applications, telles que les clients de messagerie, n’ont pas à utiliser les paramètres de EWS du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ec02f-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="ec02f-135">Les administrateurs doivent créer un compte d’emprunt d’identité pour chaque application ou une classe d’application qu’ils utilisent sur leur serveur.</span><span class="sxs-lookup"><span data-stu-id="ec02f-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="ec02f-136">Cela permettra à l’administrateur de configurer l’étendue de contrôle d’accès basé sur un rôle pour tous les utilisateurs qui n’ont pas d’autorisations EWS.</span><span class="sxs-lookup"><span data-stu-id="ec02f-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="ec02f-137">Pour activer des comptes d’emprunt d’identité, votre administrateur de serveur de test ou de production doit effectuer une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="ec02f-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="ec02f-138">Ajoutez le groupe utilisateurs authentifiés au groupe accès Compatible pré-Win2K.</span><span class="sxs-lookup"><span data-stu-id="ec02f-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="ec02f-139">Ajoutez le groupe de serveurs Exchange pour le groupe d’accès d’autorisation Windows.</span><span class="sxs-lookup"><span data-stu-id="ec02f-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="ec02f-140">Applets de commande Exchange Management Shell pour la gestion des accès</span><span class="sxs-lookup"><span data-stu-id="ec02f-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="ec02f-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="ec02f-141"></span></span>

<span data-ttu-id="ec02f-142">Les administrateurs utiliser les applets de commande Exchange Management Shell suivante pour configurer les contrôles d’accès EWS :</span><span class="sxs-lookup"><span data-stu-id="ec02f-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="ec02f-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="ec02f-143">Get-CASMailbox</span></span>](http://technet.microsoft.com/en-us/library/bb124754.aspx)
    
- [<span data-ttu-id="ec02f-144">Set-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="ec02f-144">Set-CASMailbox</span></span>](http://technet.microsoft.com/en-us/library/bb125264.aspx)
    
- [<span data-ttu-id="ec02f-145">Get-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="ec02f-145">Get-OrganizationConfig</span></span>](http://technet.microsoft.com/en-us/library/aa997571.aspx)
    
- [<span data-ttu-id="ec02f-146">Set-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="ec02f-146">Set-OrganizationConfig</span></span>](http://technet.microsoft.com/en-us/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="ec02f-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec02f-147">See also</span></span>

- [<span data-ttu-id="ec02f-148">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec02f-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="ec02f-149">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec02f-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="ec02f-150">Exchange Server PowerShell (Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="ec02f-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="ec02f-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="ec02f-151">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

