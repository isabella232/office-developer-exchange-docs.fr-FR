---
title: Agents de transport dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Trouvez des informations sur les agents de transport dans Exchange 2013.
ms.openlocfilehash: 62fb259672c47242a57b939deb4887e1e5519e2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461757"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="596a7-103">Agents de transport dans Exchange</span><span class="sxs-lookup"><span data-stu-id="596a7-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="596a7-104">Exchange 2013 fournit une bibliothèque de classes qui prennent en charge l’extension du comportement de transport Exchange et qui permettent la lecture, l’écriture et la conversion de types de contenu.</span><span class="sxs-lookup"><span data-stu-id="596a7-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="596a7-105">Vous pouvez utiliser ces classes pour créer des applications de transport Exchange qui lisent, écrivent et traitent des messages dans le pipeline de transport.</span><span class="sxs-lookup"><span data-stu-id="596a7-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="596a7-106">Ce que vous devez savoir sur les agents de transport</span><span class="sxs-lookup"><span data-stu-id="596a7-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="596a7-107">Si vous vous posez des informations sur...</span><span class="sxs-lookup"><span data-stu-id="596a7-107">If you're wondering about…</span></span>|<span data-ttu-id="596a7-108">Voici la réponse</span><span class="sxs-lookup"><span data-stu-id="596a7-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="596a7-109">Disponibilité</span><span class="sxs-lookup"><span data-stu-id="596a7-109">Availability</span></span>  <br/> |<span data-ttu-id="596a7-110">Les agents de transport sont disponibles dans les versions d’Exchange à partir d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="596a7-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="596a7-111">Les agents de transport ne sont pas pris en charge dans Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="596a7-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="596a7-112">Utilisation à distance</span><span class="sxs-lookup"><span data-stu-id="596a7-112">Remote usage</span></span>  <br/> |<span data-ttu-id="596a7-113">Les agents de transport s’exécutent sur le serveur Exchange et ne prennent pas en charge l’utilisation à distance.</span><span class="sxs-lookup"><span data-stu-id="596a7-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="596a7-114">Les langages pris en charge</span><span class="sxs-lookup"><span data-stu-id="596a7-114">Languages supported</span></span>  <br/> |<span data-ttu-id="596a7-115">Vous pouvez utiliser n’importe quel langage .NET Framework pour utiliser des agents de transport.</span><span class="sxs-lookup"><span data-stu-id="596a7-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="596a7-116">Les outils de test et de débogage disponibles</span><span class="sxs-lookup"><span data-stu-id="596a7-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="596a7-117">Utilisez des versions de Visual Studio à partir de Visual Studio 2012 pour déboguer des agents de transport.</span><span class="sxs-lookup"><span data-stu-id="596a7-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="596a7-118">Méthodes de déploiement</span><span class="sxs-lookup"><span data-stu-id="596a7-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="596a7-119">Vous pouvez installer les applications d’agent de transport à l’aide d’un script [Exchange Management Shell](../management/exchange-management-shell.md) .</span><span class="sxs-lookup"><span data-stu-id="596a7-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="596a7-120">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="596a7-120">In this section</span></span>

- [<span data-ttu-id="596a7-121">API de l’agent de transport nouvelles et mises à jour dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="596a7-122">Exemples de code de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="596a7-123">Concepts sur les agents de transport dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="596a7-124">Lecture et modification de messages dans le pipeline de transport Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="596a7-125">Création d’agents de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="596a7-126">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="596a7-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="596a7-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="596a7-127">See also</span></span>

- [<span data-ttu-id="596a7-128">Développement d’Exchange et Exchange Online</span><span class="sxs-lookup"><span data-stu-id="596a7-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="596a7-129">Explorer l'API managée EWS, EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="596a7-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="596a7-130">Sauvegarde et restauration pour Exchange</span><span class="sxs-lookup"><span data-stu-id="596a7-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

