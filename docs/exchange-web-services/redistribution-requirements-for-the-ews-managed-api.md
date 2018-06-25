---
title: Configuration requise de redistribution pour l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Découvrez comment vous pouvez redistribuer les assemblys d’API managées avec votre application.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755062"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="d2c23-103">Configuration requise de redistribution pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="d2c23-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="d2c23-104">Découvrez comment vous pouvez redistribuer les assemblys d’API managées avec votre application.</span><span class="sxs-lookup"><span data-stu-id="d2c23-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="d2c23-105">Lorsque vous concevez votre application d’API managées, vous souhaiterez également à prendre en compte la façon dont vous serez la version à vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d2c23-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="d2c23-106">Redistribution votre application d’API managées</span><span class="sxs-lookup"><span data-stu-id="d2c23-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="d2c23-107">Sauf si votre application se trouve sur le serveur Exchange, vous devrez redistribuer les assemblys d’API managées.</span><span class="sxs-lookup"><span data-stu-id="d2c23-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="d2c23-108">Le téléchargement d’API managées contient deux assemblys que vous pouvez redistribuer : Microsoft.Exchange.WebServices.dll et Microsoft.Exchange.WebServices.Auth.dll.</span><span class="sxs-lookup"><span data-stu-id="d2c23-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="d2c23-109">Gardez les informations suivantes à l’esprit lorsque vous concevez comment vous libère votre application d’API managées :</span><span class="sxs-lookup"><span data-stu-id="d2c23-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="d2c23-110">L’API managée EWS a été conçu de sorte que vous pouvez télécharger et distribuer avec votre application ciblant un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2c23-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="d2c23-111">Autrement, votre application peut télécharger l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="d2c23-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="d2c23-112">Vous pouvez utiliser l’API managée EWS pour communiquer avec un serveur Exchange exécutant Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="d2c23-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="d2c23-113">Dans les versions de l’API managée EWS depuis la version 2.1, vous pouvez installer l’API dans le Global Assembly Cache (GAC).</span><span class="sxs-lookup"><span data-stu-id="d2c23-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="d2c23-114">Le fichier MSI ajoute automatiquement la DLL dans le GAC et est accessible sur chaque ordinateur, et non sur chaque utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d2c23-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="d2c23-115">Les termes du contrat de licence est inclus dans le téléchargement d’API managées.</span><span class="sxs-lookup"><span data-stu-id="d2c23-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="d2c23-116">Passez en revue les termes pour les informations de référence sur ce que vous pouvez faire avec l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="d2c23-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d2c23-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2c23-117">See also</span></span>


- [<span data-ttu-id="d2c23-118">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d2c23-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="d2c23-119">API managée EWS (télécharger)</span><span class="sxs-lookup"><span data-stu-id="d2c23-119">EWS Managed API (download)</span></span>](http://aka.ms/ews-managed-api-readme)
    

