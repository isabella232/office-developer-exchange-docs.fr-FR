---
title: Contrôler l’accès à EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Découvrez comment contrôler l’accès à EWS pour les utilisateurs, les applications ou l’ensemble de l’organisation.
localization_priority: Priority
ms.openlocfilehash: bd65b099ab15c1514945d8a1cfa4e9b1428a4755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456877"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="d0573-103">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d0573-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="d0573-104">Découvrez comment contrôler l’accès à EWS pour les utilisateurs, les applications ou l’ensemble de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="d0573-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="d0573-105">Que vous utilisiez l’API managée EWS ou EWS directement, dans votre application, vous pouvez contrôler l’accès aux services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d0573-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="d0573-106">Si vous disposez d’un accès administrateur à votre serveur Exchange, vous pouvez gérer l’accès à EWS à l’aide de l’environnement de commande Exchange Management Shell pour contrôler l’accès au niveau global, pour chaque utilisateur et pour chaque application.</span><span class="sxs-lookup"><span data-stu-id="d0573-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="d0573-107">Applets de commande Exchange Management Shell pour la configuration du contrôle d’accès</span><span class="sxs-lookup"><span data-stu-id="d0573-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="d0573-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="d0573-108"><a name="bk_Cmdlets"> </a></span></span>

<span data-ttu-id="d0573-109">Vous pouvez utiliser les cmdlets de l’environnement de commande Exchange Management Shell suivantes pour afficher la configuration d’accès actuelle et définir les contrôles d’accès EWS :</span><span class="sxs-lookup"><span data-stu-id="d0573-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="d0573-110">[Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) -vous indique quels paramètres sont définis pour une boîte aux lettres particulière.</span><span class="sxs-lookup"><span data-stu-id="d0573-110">[Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="d0573-111">[Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) : définit les paramètres d’une boîte aux lettres particulière.</span><span class="sxs-lookup"><span data-stu-id="d0573-111">[Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="d0573-112">[Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) -affiche les paramètres de l’ensemble de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="d0573-112">[Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="d0573-113">[Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) -définit les paramètres pour l’ensemble de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="d0573-113">[Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="d0573-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="d0573-114"><a name="bk_Examples"> </a></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="d0573-115">Exemples : contrôler l’accès à EWS</span><span class="sxs-lookup"><span data-stu-id="d0573-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="d0573-116">Examinons quelques scénarios qui vous montrent comment vous pouvez contrôler l’accès à votre application.</span><span class="sxs-lookup"><span data-stu-id="d0573-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="d0573-117">**Tableau 1. Commandes permettant de contrôler l’accès à EWS**</span><span class="sxs-lookup"><span data-stu-id="d0573-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="d0573-118">Si vous souhaitez...</span><span class="sxs-lookup"><span data-stu-id="d0573-118">If you want to</span></span> |<span data-ttu-id="d0573-119">Utilisez cette commande</span><span class="sxs-lookup"><span data-stu-id="d0573-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0573-120">Bloquer toutes les applications clientes à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="d0573-121">Cela permet aux applications figurant dans le AllowList de se connecter.</span><span class="sxs-lookup"><span data-stu-id="d0573-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="d0573-122">Dans cet exemple, aucune application n’est incluse dans le AllowList, de sorte qu’aucune application ne puisse utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="d0573-123">Autoriser une liste d’applications clientes à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="d0573-124">Cela permet à des applications spécifiques d’utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="d0573-125">Dans cet exemple, toute application dont la chaîne de l’agent utilisateur commence par « OWA/ » est autorisée à accéder.</span><span class="sxs-lookup"><span data-stu-id="d0573-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="d0573-126">Autorisez toutes les applications clientes à utiliser EWS, sauf celles qui sont spécifiquement bloquées.</span><span class="sxs-lookup"><span data-stu-id="d0573-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="d0573-127">Cet exemple empêche uniquement les applications d’utiliser EWS qui ont une chaîne d’agent utilisateur qui commence par « OWA/ ».</span><span class="sxs-lookup"><span data-stu-id="d0573-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="d0573-128">Autorisez toutes les applications clientes à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="d0573-129">Aucune application de blocage n’étant spécifiée, toutes les applications peuvent utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="d0573-130">Bloquer l’ensemble de l’organisation à l’aide d’EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="d0573-131">Autorisez l’ensemble de l’organisation à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="d0573-132">Bloquer une boîte aux lettres individuelle à partir d’EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="d0573-133">Autoriser une boîte aux lettres individuelle à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="d0573-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="d0573-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0573-134">See also</span></span>

- [<span data-ttu-id="d0573-135">Configuration de votre application EWS</span><span class="sxs-lookup"><span data-stu-id="d0573-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="d0573-136">Contrôle de l'accès aux applications de client pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d0573-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="d0573-137">Exchange Server PowerShell (environnement de commande Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="d0573-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="d0573-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d0573-138">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

