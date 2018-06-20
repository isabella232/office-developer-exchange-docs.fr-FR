---
title: La configuration de votre environnement de développement d’application Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.
ms.openlocfilehash: 0c7d4c6d37b28b6797bdb638930b8582f31ffc5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755067"
---
# <a name="setting-up-your-exchange-application-development-environment"></a><span data-ttu-id="99029-103">La configuration de votre environnement de développement d’application Exchange</span><span class="sxs-lookup"><span data-stu-id="99029-103">Setting up your Exchange application development environment</span></span>

<span data-ttu-id="99029-104">Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.</span><span class="sxs-lookup"><span data-stu-id="99029-104">Learn about how to set up your development environment to create an EWS application that communicates with Exchange.</span></span>
  
<span data-ttu-id="99029-105">Avant de commencer à écrire votre application Exchange Web Services (EWS), vous devez vous assurer que votre environnement de développement présente quelques configuration minimale requise.</span><span class="sxs-lookup"><span data-stu-id="99029-105">Before you start writing your Exchange Web Services (EWS) application, you'll need to make sure that your development environment meets a few minimum requirements.</span></span> <span data-ttu-id="99029-106">Vous pouvez utiliser l’API managée EWS, l’API d’accès client standard pour les applications .NET Framework, pour développer votre application, ou vous pouvez utiliser EWS sur son propre, avec notre sans un proxy généré automatiquement.</span><span class="sxs-lookup"><span data-stu-id="99029-106">You can use the EWS Managed API, the standard client access API for .NET Framework applications, to develop your application, or you can use EWS on its own, with our without an autogenerated proxy.</span></span> <span data-ttu-id="99029-107">En général, nous vous recommandons d’utiliser l’API managée EWS ; Toutefois, vous pouvez [Explorer la différence entre ces deux options](ews-client-design-overview-for-exchange.md) plus en détail pour rechercher les est fait pour vous.</span><span class="sxs-lookup"><span data-stu-id="99029-107">In general, we recommend that you use the EWS Managed API; however, you can [explore the difference between these two options](ews-client-design-overview-for-exchange.md) in more detail to find out which one is right for you.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="99029-p102">[!REMARQUE]  L'API managée EWS est maintenant disponible en tant que projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source pour : >  participer aux résolutions de bogues et aux améliorations apportées à l'API ; >  obtenir des correctifs et des améliorations avant qu'ils soient disponibles dans une version officielle ; >  accéder à l'implémentation la plus complète et la plus à jour de l'API, afin de l'utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes. >  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub sont les bienvenues.</span><span class="sxs-lookup"><span data-stu-id="99029-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="development-environment-for-the-ews-managed-api"></a><span data-ttu-id="99029-113">Environnement de développement pour l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="99029-113">Development environment for the EWS Managed API</span></span>
<span data-ttu-id="99029-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="99029-114"></span></span>

<span data-ttu-id="99029-115">Pour créer une application d’API managées, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="99029-115">To create an EWS Managed API application, you'll need access to the following:</span></span>
  
- <span data-ttu-id="99029-116">L'[API managée EWS](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="99029-116">The [EWS Managed API](http://aka.ms/ews-managed-api-readme).</span></span> 
    
    <span data-ttu-id="99029-117">Vous pouvez stocker les fichiers de l’API managée EWS n’importe où sur votre ordinateur ; par défaut, ils sont installés dans les Services Files\Microsoft\Exchange\Web\\< numéro de version\> dossier.</span><span class="sxs-lookup"><span data-stu-id="99029-117">You can store the EWS Managed API files anywhere on your computer; by default, they are installed in the Program Files\Microsoft\Exchange\Web Services\\<version number\> folder.</span></span>
    
- <span data-ttu-id="99029-118">Une boîte aux lettres sur un serveur Exchange qui exécute Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange commençant par Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="99029-118">A mailbox on an Exchange server that is running Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange Server 2007.</span></span> 
    
    <span data-ttu-id="99029-119">Vous pouvez obtenir un plan Exchange Online pour les entreprises, y compris une version d’évaluation gratuite, à partir du [site Office 365](http://office.microsoft.com/en-us/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a).</span><span class="sxs-lookup"><span data-stu-id="99029-119">You can get an Exchange Online plan for business, including a free trial, from the [Office 365 site](http://office.microsoft.com/en-us/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a).</span></span> <span data-ttu-id="99029-120">Pour pouvoir se connecter à la boîte aux lettres, vous devez disposer du nom d’utilisateur et les informations d’identification du compte associé à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="99029-120">In order to connect to the mailbox you must have the user name and credentials of the account associated with the mailbox.</span></span>
    
- <span data-ttu-id="99029-121">Une version de Visual Studio commençant par Visual Studio 2005.</span><span class="sxs-lookup"><span data-stu-id="99029-121">A version of Visual Studio starting with Visual Studio 2005.</span></span> <span data-ttu-id="99029-122">Si vous ne disposez pas de Visual Studio, vous pouvez télécharger une version gratuite de [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).</span><span class="sxs-lookup"><span data-stu-id="99029-122">If you don't currently have Visual Studio, you can download a free version of [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).</span></span>
    
- <span data-ttu-id="99029-123">Une version du .NET Framework commençant par le .NET Framework 3.5.</span><span class="sxs-lookup"><span data-stu-id="99029-123">A version of the .NET Framework starting with the .NET Framework 3.5.</span></span> <span data-ttu-id="99029-124">Vous pouvez télécharger le .NET Framework 3.5 à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).</span><span class="sxs-lookup"><span data-stu-id="99029-124">You can download the .NET Framework 3.5 from the [Microsoft Download Center](http://go.microsoft.com/fwlink/?LinkId=191777).</span></span>
    
<span data-ttu-id="99029-125">En outre, il est utile si vous être familiarisé avec c#.</span><span class="sxs-lookup"><span data-stu-id="99029-125">In addition, it is helpful if you have some familiarity with C#.</span></span> <span data-ttu-id="99029-126">Bien que Visual Studio prend en charge les autres langues en plus de Visual C#, la plupart des exemples de code disponibles pour l’API managée EWS est écrit en c#.</span><span class="sxs-lookup"><span data-stu-id="99029-126">Although Visual Studio supports other languages in addition to C#, most of the sample code available for the EWS Managed API is written in C#.</span></span>
  
## <a name="development-environment-for-ews"></a><span data-ttu-id="99029-127">Environnement de développement pour EWS</span><span class="sxs-lookup"><span data-stu-id="99029-127">Development environment for EWS</span></span>
<span data-ttu-id="99029-128"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="99029-128"></span></span>

<span data-ttu-id="99029-129">Vous pouvez utiliser EWS pour développer votre application de deux manières différentes.</span><span class="sxs-lookup"><span data-stu-id="99029-129">You can use EWS to develop your application in a couple of different ways.</span></span> <span data-ttu-id="99029-130">La façon la plus simple d’utiliser EWS consiste à créer des fichiers texte qui contiennent des demandes de votre XML et de les transmettre à Exchange.</span><span class="sxs-lookup"><span data-stu-id="99029-130">The simplest way to use EWS is to create text files that contain your XML requests, and transmit them to Exchange.</span></span> <span data-ttu-id="99029-131">Pour ce faire, voici ce que vous devez :</span><span class="sxs-lookup"><span data-stu-id="99029-131">To do this, here is what you need:</span></span> 
  
- <span data-ttu-id="99029-132">Un simple éditeur de texte tel que le bloc-notes, pour modifier votre requête XML.</span><span class="sxs-lookup"><span data-stu-id="99029-132">A simple text editor, like Notepad, to edit your XML request.</span></span> <span data-ttu-id="99029-133">N’importe quel éditeur de texte fera, bien que vous pouvez souhaiter une qui vous aideront à votre validation de la syntaxe XML comme XMetal.</span><span class="sxs-lookup"><span data-stu-id="99029-133">Any text editor will do, although you might want one that will help with your XML syntax validation like XMetal.</span></span>
    
- <span data-ttu-id="99029-134">Un outil ou une application qui peut envoyer et recevoir des demandes SOAP XML et des réponses, afin de pouvoir communiquer avec Exchange.</span><span class="sxs-lookup"><span data-stu-id="99029-134">A tool or application that can send and receive SOAP XML requests and responses, in order to communicate with Exchange.</span></span>
    
<span data-ttu-id="99029-135">Lorsque vous travaillez avec le code XML brut, il est également utile d’avoir une connaissance élémentaire de mise en forme XML.</span><span class="sxs-lookup"><span data-stu-id="99029-135">When you work with raw XML, it's also helpful to have a basic understanding of XML formatting.</span></span>
  
<span data-ttu-id="99029-136">Utiliser EWS, la deuxième consiste à créer un proxy généré automatiquement qui vous permet de travailler avec les opérations à l’aide d’un langage .NET tel que c#.</span><span class="sxs-lookup"><span data-stu-id="99029-136">The second way to use EWS is to create an autogenerated proxy that enables you to work with the operations by using a .NET language like C#.</span></span> <span data-ttu-id="99029-137">Voici ce que vous devez utiliser un proxy généré automatiquement :</span><span class="sxs-lookup"><span data-stu-id="99029-137">Here is what you need to work with an autogenerated proxy:</span></span>
  
- <span data-ttu-id="99029-138">Une version de Visual Studio commençant par Visual Studio 2005, pour créer une référence au serveur proxy.</span><span class="sxs-lookup"><span data-stu-id="99029-138">A version of Visual Studio starting with Visual Studio 2005, to create a proxy reference.</span></span> <span data-ttu-id="99029-139">Vous pouvez télécharger une version gratuite de [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).</span><span class="sxs-lookup"><span data-stu-id="99029-139">You can download a free version of [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).</span></span>
    
- <span data-ttu-id="99029-140">Une version du .NET Framework commençant par le .NET Framework 2.0.</span><span class="sxs-lookup"><span data-stu-id="99029-140">A version of the .NET Framework starting with the .NET Framework 2.0.</span></span> <span data-ttu-id="99029-141">Vous pouvez télécharger le .NET Framework 3.5 à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).</span><span class="sxs-lookup"><span data-stu-id="99029-141">You can download the .NET Framework 3.5 from the [Microsoft Download Center](http://go.microsoft.com/fwlink/?LinkId=191777).</span></span>
    
<span data-ttu-id="99029-142">Si vous utilisez un proxy généré automatiquement, vous souhaiterez être familiarisé avec la programmation c#.</span><span class="sxs-lookup"><span data-stu-id="99029-142">If you use an autogenerated proxy, you'll want to have some familiarity with C# programming.</span></span>
  
> [!NOTE]
> <span data-ttu-id="99029-143">Si vous êtes un développeur .NET Framework, nous vous conseillons d’utiliser l’API managées plutôt que des serveurs proxy généré automatiquement pour développer avec EWS.</span><span class="sxs-lookup"><span data-stu-id="99029-143">If you're a .NET Framework developer, we encourage you to use the EWS Managed API rather than autogenerated proxies to develop against EWS.</span></span> <span data-ttu-id="99029-144">Le modèle objet d’API managées est plus facile à utiliser que les modèles objet de proxy généré automatiquement.</span><span class="sxs-lookup"><span data-stu-id="99029-144">The EWS Managed API object model is easier to use than autogenerated proxy object models.</span></span> <span data-ttu-id="99029-145">En outre, l’API managée EWS implémente la [découverte automatique](autodiscover-for-exchange.md) et inclut une logique côté client.</span><span class="sxs-lookup"><span data-stu-id="99029-145">Also, the EWS Managed API implements [Autodiscover](autodiscover-for-exchange.md) and includes client-side logic.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="99029-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="99029-146">See also</span></span>


- [<span data-ttu-id="99029-147">La configuration de votre environnement de développement d'applications Exchange</span><span class="sxs-lookup"><span data-stu-id="99029-147">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)
    
- [<span data-ttu-id="99029-148">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="99029-148">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="99029-149">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="99029-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
    
- [<span data-ttu-id="99029-150">EWS généré des modèles objet pour Exchange</span><span class="sxs-lookup"><span data-stu-id="99029-150">EWS generated object models for Exchange</span></span>](https://msdn.microsoft.com/en-us/library/jj190899)
    
