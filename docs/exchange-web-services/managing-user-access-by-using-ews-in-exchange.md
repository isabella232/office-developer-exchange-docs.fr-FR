---
title: Gestion de l’accès utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Découvrez quelles sont vos options pour la gestion de compte d’utilisateur accès à votre serveur Exchange.
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754973"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="e73a6-103">Gestion de l’accès utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e73a6-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="e73a6-104">Découvrez quelles sont vos options pour la gestion de compte d’utilisateur accès à votre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="e73a6-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="e73a6-105">API gérée d’Exchange Web Services (EWS) et le EWS fournissent un nombre limité d’opérations que vous pouvez utiliser pour gérer les comptes dans Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange commençant par Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="e73a6-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="e73a6-106">Vous pouvez utiliser les opérations indiquées dans la figure suivante pour gérer les délégués et pour définir des autorisations d’accès au dossier pour les autres comptes.</span><span class="sxs-lookup"><span data-stu-id="e73a6-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="e73a6-107">**Opérations EWS pour l’accès délégué et de dossier**</span><span class="sxs-lookup"><span data-stu-id="e73a6-107">**EWS operations for delegate and folder access**</span></span>

![Options de gestion des utilisateurs EWS.](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="e73a6-109">Si votre application a besoin d’un contrôle supplémentaire sur les comptes sur un serveur Exchange, vous pouvez utiliser les applets de commande Exchange Management Shell pour gérer les comptes.</span><span class="sxs-lookup"><span data-stu-id="e73a6-109">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts.</span></span> <span data-ttu-id="e73a6-110">Vous pouvez appeler les applets de commande Exchange Management Shell en effectuant l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="e73a6-110">You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="e73a6-111">Écriture d’une application à l’aide de c# ou Visual Basic qui appelle les applets de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="e73a6-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="e73a6-112">Vous pouvez consulter l’exemple de code dans la [documentation sur Exchange Management Shell API](../management/exchange-management-shell.md) pour découvrir comment appeler une applet de commande.</span><span class="sxs-lookup"><span data-stu-id="e73a6-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="e73a6-113">À l’aide de Windows PowerShell et les scripts Windows PowerShell pour appeler les applets de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="e73a6-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="e73a6-114">Vous trouverez une liste complète de la [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), ainsi que des exemples qui montrent comment les utiliser.</span><span class="sxs-lookup"><span data-stu-id="e73a6-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="e73a6-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e73a6-115">See also</span></span>

- [<span data-ttu-id="e73a6-116">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="e73a6-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="e73a6-117">Applets de commande Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e73a6-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

