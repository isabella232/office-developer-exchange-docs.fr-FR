---
title: Contrôle de l'accès aux applications de client pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Découvrez les options permettant de gérer l’accès des applications clientes à EWS.
localization_priority: Priority
ms.openlocfilehash: b887b8167e3d38946b1d6caffe12655ded89569f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528460"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="1a917-103">Contrôle de l'accès aux applications de client pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a917-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="1a917-104">Découvrez les options permettant de gérer l’accès des applications clientes à EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="1a917-105">Toute application cliente EWS que vous créez doit disposer d’un accès à Exchange Online, Exchange Online dans le cadre d’Office 365 ou de la version d’Exchange à partir d’Exchange 2013 avant de pouvoir appeler les opérations EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="1a917-106">Les administrateurs de serveurs de test ou de production peuvent utiliser l’environnement de commande Exchange Management Shell pour limiter l’accès à EWS pour tous les utilisateurs et toutes les applications, pour des utilisateurs individuels ou pour des applications individuelles.</span><span class="sxs-lookup"><span data-stu-id="1a917-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="1a917-107">Le contrôle d’accès pour EWS est basé sur les comptes de domaine.</span><span class="sxs-lookup"><span data-stu-id="1a917-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="1a917-108">Lorsqu’une connexion est établie avec des informations d’identification authentifiées par l’autorité de sécurité locale, le serveur renvoie une erreur qui indique que seuls les comptes de domaine peuvent se connecter.</span><span class="sxs-lookup"><span data-stu-id="1a917-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="1a917-109">Contrôle d’accès pour les clients et les utilisateurs EWS</span><span class="sxs-lookup"><span data-stu-id="1a917-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="1a917-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="1a917-110"><a name="bk_configure"> </a></span></span>

<span data-ttu-id="1a917-111">Votre administrateur de serveur de test ou de production peut configurer le contrôle d’accès pour les clients qui se connectent à EWS de l’une des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="1a917-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="1a917-112">En bloquant toutes les applications clientes de se connecter.</span><span class="sxs-lookup"><span data-stu-id="1a917-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="1a917-113">En autorisant des applications clientes spécifiques à se connecter uniquement.</span><span class="sxs-lookup"><span data-stu-id="1a917-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="1a917-114">En autorisant toute application cliente à se connecter à l’exception de celles qui sont spécifiquement bloquées.</span><span class="sxs-lookup"><span data-stu-id="1a917-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="1a917-115">En autorisant toute application cliente à se connecter.</span><span class="sxs-lookup"><span data-stu-id="1a917-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="1a917-116">Les applications sont identifiées par la chaîne de l’agent utilisateur qu’elles envoient dans la requête Web HTTP.</span><span class="sxs-lookup"><span data-stu-id="1a917-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="1a917-117">Le blocage au niveau de l’application n’est pas une fonctionnalité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="1a917-117">Application-level blocking is not a security feature.</span></span> <span data-ttu-id="1a917-118">La chaîne de l’agent utilisateur est facilement usurpée.</span><span class="sxs-lookup"><span data-stu-id="1a917-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="1a917-119">Si une application est autorisée à accéder à EWS, elle doit toujours présenter les informations d’identification que le serveur authentifie avant que l’application ne puisse se connecter à EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="1a917-120">Les administrateurs peuvent également configurer le contrôle d’accès pour les propriétaires de boîtes aux lettres qui se connectent à EWS de la manière suivante :</span><span class="sxs-lookup"><span data-stu-id="1a917-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="1a917-121">En bloquant ou en autorisant une organisation entière.</span><span class="sxs-lookup"><span data-stu-id="1a917-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="1a917-122">En bloquant ou en autorisant un groupe d’utilisateurs identifié par une étendue d’authentification basée sur un rôle qui inclut ou exclut les propriétaires de boîtes aux lettres qui n’ont pas accès à EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="1a917-123">En bloquant ou en autorisant un propriétaire de boîte aux lettres individuelle.</span><span class="sxs-lookup"><span data-stu-id="1a917-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="1a917-124">Les paramètres de contrôle d’accès spécifiques remplacent les paramètres de contrôle d’accès généraux.</span><span class="sxs-lookup"><span data-stu-id="1a917-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="1a917-125">Par exemple, si une organisation refuse l’accès EWS mais qu’un propriétaire de boîte aux lettres individuel est autorisé à accéder aux applications, le paramètre individuel est prioritaire et l’accès est autorisé.</span><span class="sxs-lookup"><span data-stu-id="1a917-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="1a917-126">Délégation et gestion de l’accès EWS</span><span class="sxs-lookup"><span data-stu-id="1a917-126">Delegation and EWS access management</span></span>
<span data-ttu-id="1a917-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="1a917-127"><a name="bk_delegation"> </a></span></span>

<span data-ttu-id="1a917-128">Lorsque les utilisateurs délégués qui n’ont pas accès à EWS utilisent votre application cliente, ils ne pourront pas accéder à la boîte aux lettres de l’utilisateur principal à l’aide d’EWS, même si l’utilisateur principal dispose d’un accès EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="1a917-129">Si l’utilisateur délégué dispose d’un accès EWS, le délégué pourra utiliser votre application cliente EWS pour accéder à la boîte aux lettres de l’utilisateur principal même si l’utilisateur principal ne dispose pas d’un accès EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="1a917-130">Emprunt d’identité et gestion des accès EWS</span><span class="sxs-lookup"><span data-stu-id="1a917-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="1a917-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="1a917-131"><a name="bk_impersonation"> </a></span></span>

<span data-ttu-id="1a917-132">Les applications clientes qui se connectent à EWS pour le compte de propriétaires de boîtes aux lettres risquent de ne pas pouvoir utiliser les paramètres EWS du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a917-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="1a917-133">Par exemple, une application qui archive les messages électroniques d’une société doit se connecter à EWS indépendamment de ce que sont les paramètres des utilisateurs de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a917-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="1a917-134">D’autres applications, telles que les clients de messagerie, doivent utiliser les paramètres EWS du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1a917-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="1a917-135">Les administrateurs doivent créer un compte d’emprunt d’identité pour chaque application ou classe d’application qu’ils utilisent sur leur serveur.</span><span class="sxs-lookup"><span data-stu-id="1a917-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="1a917-136">Cela permet à l’administrateur de configurer l’étendue de contrôle d’accès basée sur un rôle pour tous les utilisateurs qui ne disposent pas d’autorisations EWS.</span><span class="sxs-lookup"><span data-stu-id="1a917-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="1a917-137">Pour activer les comptes d’emprunt d’identité, votre administrateur de serveur de test ou de production doit effectuer l’une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="1a917-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="1a917-138">Ajoutez le groupe utilisateurs authentifiés au groupe d’accès compatible pré-Win2K.</span><span class="sxs-lookup"><span data-stu-id="1a917-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="1a917-139">Ajoutez le groupe serveurs Exchange au groupe d’accès d’autorisation Windows.</span><span class="sxs-lookup"><span data-stu-id="1a917-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="1a917-140">Applets de commande Exchange Management Shell pour la gestion des accès</span><span class="sxs-lookup"><span data-stu-id="1a917-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="1a917-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="1a917-141"><a name="bk_cmdlets"> </a></span></span>

<span data-ttu-id="1a917-142">Les administrateurs utilisent les cmdlets Exchange Management Shell suivantes pour configurer les contrôles d’accès EWS :</span><span class="sxs-lookup"><span data-stu-id="1a917-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="1a917-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="1a917-143">Get-CASMailbox</span></span>](https://technet.microsoft.com/library/bb124754.aspx)   
- [<span data-ttu-id="1a917-144">Set-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="1a917-144">Set-CASMailbox</span></span>](https://technet.microsoft.com/library/bb125264.aspx)   
- [<span data-ttu-id="1a917-145">Get-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="1a917-145">Get-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997571.aspx)   
- [<span data-ttu-id="1a917-146">Set-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="1a917-146">Set-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="1a917-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a917-147">See also</span></span>

- [<span data-ttu-id="1a917-148">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a917-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="1a917-149">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a917-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="1a917-150">Exchange Server PowerShell (environnement de commande Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="1a917-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="1a917-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="1a917-151">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

