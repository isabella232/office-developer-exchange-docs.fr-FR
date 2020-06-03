---
title: Besoins de redistribution pour l'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Découvrez comment vous pouvez redistribuer les assemblys d’API managée EWS avec votre application.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463824"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="7d809-103">Besoins de redistribution pour l'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7d809-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="7d809-104">Découvrez comment vous pouvez redistribuer les assemblys d’API managée EWS avec votre application.</span><span class="sxs-lookup"><span data-stu-id="7d809-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="7d809-105">Lors de la conception de votre application d’API managée EWS, vous devez également prendre en compte la manière dont vous allez la libérer pour vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="7d809-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="7d809-106">Redistribution de votre application d’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7d809-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="7d809-107">À moins que votre application se trouve sur le serveur Exchange, vous devrez redistribuer les assemblys de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7d809-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="7d809-108">Le téléchargement de l’API managée EWS contient deux assemblys que vous pouvez redistribuer : Microsoft. Exchange. WebServices. dll et Microsoft. Exchange. WebServices. auth. dll.</span><span class="sxs-lookup"><span data-stu-id="7d809-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="7d809-109">Gardez les informations suivantes à l’esprit lors de la conception de votre application d’API managée EWS :</span><span class="sxs-lookup"><span data-stu-id="7d809-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="7d809-110">L’API managée EWS a été conçue de sorte que vous pouvez la télécharger et la distribuer avec votre application qui cible un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d809-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="7d809-111">Par ailleurs, votre application peut télécharger l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7d809-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="7d809-112">Vous pouvez utiliser l’API managée EWS pour communiquer avec un serveur Exchange exécutant Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="7d809-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="7d809-113">Dans les versions de l’API managée EWS à partir de la version 2,1, vous pouvez installer l’API dans le global assembly cache (GAC).</span><span class="sxs-lookup"><span data-stu-id="7d809-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="7d809-114">Le MSI ajoutera automatiquement la DLL au GAC et sera accessible par ordinateur, et non par utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7d809-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="7d809-115">Les termes du contrat de licence sont inclus dans le téléchargement de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7d809-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="7d809-116">Passez en revue les termes des informations faisant autorité sur ce que vous pouvez faire avec l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7d809-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7d809-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d809-117">See also</span></span>


- [<span data-ttu-id="7d809-118">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7d809-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="7d809-119">API managée EWS (téléchargement)</span><span class="sxs-lookup"><span data-stu-id="7d809-119">EWS Managed API (download)</span></span>](https://aka.ms/ews-managed-api-readme)
    

