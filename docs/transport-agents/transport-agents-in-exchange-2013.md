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
ms.openlocfilehash: 1a28ae79e2a7e338ddd6cb1f6961dd14a980b56e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755145"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="5e443-103">Agents de transport dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5e443-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="5e443-104">Exchange 2013 fournit une bibliothèque de classes qui prennent en charge l’extension du comportement de transport Exchange et activer la lecture, écriture et la conversion des types de contenu.</span><span class="sxs-lookup"><span data-stu-id="5e443-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="5e443-105">Vous pouvez utiliser ces classes pour créer des applications de transport Exchange lire, écrivent et traitent les messages dans le pipeline de transport.</span><span class="sxs-lookup"><span data-stu-id="5e443-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="5e443-106">Vous devez savoir à propos des agents de transport</span><span class="sxs-lookup"><span data-stu-id="5e443-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="5e443-107">Si vous vous interrogez sur...</span><span class="sxs-lookup"><span data-stu-id="5e443-107">If you're wondering about…</span></span>|<span data-ttu-id="5e443-108">Voici la réponse</span><span class="sxs-lookup"><span data-stu-id="5e443-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e443-109">Disponibilité</span><span class="sxs-lookup"><span data-stu-id="5e443-109">Availability</span></span>  <br/> |<span data-ttu-id="5e443-110">Agents de transport sont disponibles dans les versions d’Exchange commençant par Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="5e443-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="5e443-111">Agents de transport ne sont pas pris en charge dans Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5e443-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="5e443-112">Utilisation à distance</span><span class="sxs-lookup"><span data-stu-id="5e443-112">Remote usage</span></span>  <br/> |<span data-ttu-id="5e443-113">Agents de transport s’exécutent sur le serveur Exchange et ne prennent pas en charge l’utilisation à distance.</span><span class="sxs-lookup"><span data-stu-id="5e443-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="5e443-114">Les langages pris en charge</span><span class="sxs-lookup"><span data-stu-id="5e443-114">Languages supported</span></span>  <br/> |<span data-ttu-id="5e443-115">Vous pouvez utiliser n’importe quel langage .NET Framework pour travailler avec des agents de transport.</span><span class="sxs-lookup"><span data-stu-id="5e443-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="5e443-116">Les outils de test et de débogage disponibles</span><span class="sxs-lookup"><span data-stu-id="5e443-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="5e443-117">Utiliser les versions de Visual Studio commençant par Visual Studio 2012 pour déboguer des agents de transport.</span><span class="sxs-lookup"><span data-stu-id="5e443-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="5e443-118">Méthodes de déploiement</span><span class="sxs-lookup"><span data-stu-id="5e443-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="5e443-119">Vous pouvez installer des applications de l’agent de transport à l’aide d’un script [Exchange Management Shell](../management/exchange-management-shell.md) .</span><span class="sxs-lookup"><span data-stu-id="5e443-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="5e443-120">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="5e443-120">In this section</span></span>

- [<span data-ttu-id="5e443-121">Agent de transport nouveaux et mis à jour l’API d’Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5e443-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="5e443-122">Exemples de code de l’agent pour Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="5e443-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="5e443-123">Concepts de l’agent d’Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="5e443-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="5e443-124">Lecture et de modification des messages dans le pipeline de transport Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5e443-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="5e443-125">Création d’agents de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5e443-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="5e443-126">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5e443-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="5e443-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5e443-127">See also</span></span>

- [<span data-ttu-id="5e443-128">Exchange Online et développement Exchange</span><span class="sxs-lookup"><span data-stu-id="5e443-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="5e443-129">Explorer l'API managée EWS, EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5e443-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="5e443-130">Sauvegarde et restauration pour Exchange</span><span class="sxs-lookup"><span data-stu-id="5e443-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

