---
title: Gestion de l’accès des utilisateurs à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Découvrez les options disponibles pour la gestion de l’accès aux comptes d’utilisateurs à votre serveur Exchange.
ms.openlocfilehash: 476292d4db206f22cd84134ce2b46957e9fe85fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456242"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="7784c-103">Gestion de l’accès des utilisateurs à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7784c-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="7784c-104">Découvrez les options disponibles pour la gestion de l’accès aux comptes d’utilisateurs à votre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7784c-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="7784c-105">Les services Web Exchange (EWS) et l’API managée EWS fournissent un nombre limité d’opérations que vous pouvez utiliser pour gérer les comptes sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange à partir d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="7784c-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="7784c-106">Vous pouvez utiliser les opérations illustrées dans la figure suivante pour gérer les délégués et définir des autorisations d’accès aux dossiers pour d’autres comptes.</span><span class="sxs-lookup"><span data-stu-id="7784c-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="7784c-107">**Opérations EWS pour l’accès aux délégués et aux dossiers**</span><span class="sxs-lookup"><span data-stu-id="7784c-107">**EWS operations for delegate and folder access**</span></span>

![Options de gestion des utilisateurs EWS.](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="7784c-109">Si votre application a besoin d’un contrôle supplémentaire sur les comptes sur un serveur Exchange, vous pouvez utiliser les cmdlets Exchange Management Shell pour gérer les comptes.</span><span class="sxs-lookup"><span data-stu-id="7784c-109">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts.</span></span> <span data-ttu-id="7784c-110">Vous pouvez appeler les cmdlets de l’environnement de commande Exchange Management Shell en effectuant l’une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="7784c-110">You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="7784c-111">Écriture d’une application à l’aide de C# ou de Visual Basic qui appelle les cmdlets de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="7784c-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="7784c-112">Vous pouvez consulter l’exemple de code de la documentation de l’API de l’environnement de commande [Exchange Management Shell](../management/exchange-management-shell.md) pour savoir comment appeler une cmdlet.</span><span class="sxs-lookup"><span data-stu-id="7784c-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="7784c-113">Utilisation de scripts Windows PowerShell et Windows PowerShell pour appeler des applets de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="7784c-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="7784c-114">Vous trouverez une liste complète d' [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), ainsi que des exemples qui montrent comment les utiliser.</span><span class="sxs-lookup"><span data-stu-id="7784c-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="7784c-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7784c-115">See also</span></span>

- [<span data-ttu-id="7784c-116">Configuration de votre application EWS</span><span class="sxs-lookup"><span data-stu-id="7784c-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="7784c-117">Applets de commande Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7784c-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

