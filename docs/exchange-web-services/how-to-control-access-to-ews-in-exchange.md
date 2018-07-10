---
title: Contrôler l’accès à EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Découvrez comment contrôler l’accès à EWS pour les utilisateurs, des applications ou l’organisation toute entière.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754812"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="22dfe-103">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="22dfe-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="22dfe-104">Découvrez comment contrôler l’accès à EWS pour les utilisateurs, des applications ou l’organisation toute entière.</span><span class="sxs-lookup"><span data-stu-id="22dfe-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="22dfe-105">Si vous utilisez l’API managée EWS ou EWS directement dans votre application, vous pouvez contrôler l’accès à Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="22dfe-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="22dfe-106">Si vous avez accès d’administrateur sur votre serveur Exchange, vous pouvez gérer l’accès aux EWS à l’aide de l’environnement Exchange Management Shell pour contrôler l’accès au niveau global, pour chaque utilisateur et pour chaque application.</span><span class="sxs-lookup"><span data-stu-id="22dfe-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="22dfe-107">Applets de commande Exchange Management Shell pour configurer le contrôle d’accès</span><span class="sxs-lookup"><span data-stu-id="22dfe-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="22dfe-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="22dfe-108"></span></span>

<span data-ttu-id="22dfe-109">Vous pouvez utiliser les applets de commande Exchange Management Shell suivante pour afficher la configuration d’accès actuel et définir des contrôles d’accès EWS :</span><span class="sxs-lookup"><span data-stu-id="22dfe-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="22dfe-110">[Get-CASMailbox](http://technet.microsoft.com/fr-fr/library/bb124754.aspx) - affiche les paramètres sont définis pour une boîte aux lettres spécifique.</span><span class="sxs-lookup"><span data-stu-id="22dfe-110">[Get-CASMailbox](http://technet.microsoft.com/fr-fr/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="22dfe-111">[Set-CASMailbox](http://technet.microsoft.com/fr-fr/library/bb125264.aspx) - paramètres ensembles pour une boîte aux lettres spécifique.</span><span class="sxs-lookup"><span data-stu-id="22dfe-111">[Set-CASMailbox](http://technet.microsoft.com/fr-fr/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="22dfe-112">[Get-OrganizationConfig](http://technet.microsoft.com/fr-fr/library/aa997571.aspx) - affiche les paramètres de l’organisation toute entière.</span><span class="sxs-lookup"><span data-stu-id="22dfe-112">[Get-OrganizationConfig](http://technet.microsoft.com/fr-fr/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="22dfe-113">[Set-OrganizationConfig](http://technet.microsoft.com/fr-fr/library/aa997443.aspx) - définit les paramètres de l’organisation toute entière.</span><span class="sxs-lookup"><span data-stu-id="22dfe-113">[Set-OrganizationConfig](http://technet.microsoft.com/fr-fr/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="22dfe-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="22dfe-114"></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="22dfe-115">Exemples : Contrôler l’accès à EWS</span><span class="sxs-lookup"><span data-stu-id="22dfe-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="22dfe-116">Examinons quelques scénarios qui montrent comment vous pouvez contrôler l’accès à votre application.</span><span class="sxs-lookup"><span data-stu-id="22dfe-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="22dfe-117">**Le tableau 1. Commandes pour contrôler l’accès à EWS**</span><span class="sxs-lookup"><span data-stu-id="22dfe-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="22dfe-118">Si vous souhaitez</span><span class="sxs-lookup"><span data-stu-id="22dfe-118">If you want to</span></span> |<span data-ttu-id="22dfe-119">Utilisez cette commande</span><span class="sxs-lookup"><span data-stu-id="22dfe-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="22dfe-120">Bloquer toutes les applications clientes d’utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="22dfe-121">Cela permet aux applications répertoriées dans le AllowList pour se connecter.</span><span class="sxs-lookup"><span data-stu-id="22dfe-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="22dfe-122">Dans cet exemple, aucune application n’est incluse dans le AllowList, aucune application peut utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="22dfe-123">Autoriser une liste de client applications afin d’utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="22dfe-124">Cela permet à des applications spécifiques à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="22dfe-125">Dans cet exemple, n’importe quelle application qui a un agent utilisateur de chaîne qui commence par « OWA / » est autorisé à accéder.</span><span class="sxs-lookup"><span data-stu-id="22dfe-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="22dfe-126">Autoriser toutes les applications clientes à utiliser EWS, à l’exception de ceux qui sont spécifiquement bloqués.</span><span class="sxs-lookup"><span data-stu-id="22dfe-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="22dfe-127">Cet exemple montre comment bloque uniquement les applications à l’aide de EWS ayant une chaîne d’agent utilisateur qui commence par « OWA / ».</span><span class="sxs-lookup"><span data-stu-id="22dfe-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="22dfe-128">Autoriser toutes les applications clientes à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="22dfe-129">Étant donné qu’aucune liste de blocage n’est spécifié, toutes les applications peuvent utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="22dfe-130">Bloquer l’organisation toute entière à partir de l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="22dfe-131">Autoriser l’organisation toute entière à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="22dfe-132">Bloquer une boîte aux lettres à partir de l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="22dfe-133">Autoriser une boîte aux lettres à utiliser EWS.</span><span class="sxs-lookup"><span data-stu-id="22dfe-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="22dfe-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22dfe-134">See also</span></span>

- [<span data-ttu-id="22dfe-135">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="22dfe-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="22dfe-136">Contrôle de l'accès aux applications de client pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="22dfe-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="22dfe-137">Exchange Server PowerShell (Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="22dfe-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/fr-fr/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="22dfe-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="22dfe-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/fr-fr/library/dd835506%28v=vs.85%29.aspx)
    

