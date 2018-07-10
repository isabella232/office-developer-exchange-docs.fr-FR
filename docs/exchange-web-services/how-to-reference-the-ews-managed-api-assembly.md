---
title: Référence de l’assembly de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment référencer l'assembly API managée EWS.
ms.openlocfilehash: af7b1ec449c24e7fa4db89abb30e5ebc9f8d329e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754929"
---
# <a name="reference-the-ews-managed-api-assembly"></a><span data-ttu-id="7ce64-103">Référence de l’assembly de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7ce64-103">Reference the EWS Managed API assembly</span></span>

<span data-ttu-id="7ce64-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment référencer l'assembly API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7ce64-104">Find information about how to reference the EWS Managed API assembly.</span></span>
  
<span data-ttu-id="7ce64-p101">L'API managée EWS fournit une interface simple et complète pour développer et étendre les applications qui utilisent les services web Exchange (EWS). Que vous utilisiez Visual Studio ou un autre éditeur de code pour développer votre application API managée EWS, vous aurez besoin de faire référence à l'assembly API managée EWS. Si vous n'avez pas encore installé l'API managée EWS, [téléchargez-la](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="7ce64-p101">The EWS Managed API provides a simple and full-featured interface for developing and extending applications that use Exchange Web Services (EWS). Whether you are using Visual Studio or another code editor to develop your EWS Managed API application, you will need to make a reference to the EWS Managed API assembly. If you haven't installed the EWS Managed API already, be sure to [download the API](http://aka.ms/ews-managed-api-readme).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="7ce64-p102"> L'API managée EWS est maintenant disponible en tant que projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source afin de : >  participer aux résolutions de bogues et aux améliorations apportées à l'API ; >  obtenir des correctifs et des améliorations avant qu'ils soient disponibles dans une version officielle ; >  accéder à l'implémentation la plus complète et la plus à jour de l'API, afin de l'utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes. >  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub sont les bienvenues.</span><span class="sxs-lookup"><span data-stu-id="7ce64-p102">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api). You can use the open source library to: >  Contribute bug fixes and enhancements to the API. >  Get fixes and enhancements before they are available in an official release. >  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms. >  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="referencing-the-assembly"></a><span data-ttu-id="7ce64-113">Référencement de l'assembly</span><span class="sxs-lookup"><span data-stu-id="7ce64-113">Referencing the assembly</span></span>

<span data-ttu-id="7ce64-p103">La façon la plus courante d'ajouter une référence est d'utiliser Visual Studio. Nous savons que certains développeurs préfèrent utiliser d'autres éditeurs, donc nous allons vous donner des instructions pour utiliser le compilateur de ligne de commande, ainsi que des instructions pour l'utilisation de Visual Studio. Vous remarquerez que les exemples de code qui suivent présentent les mêmes instructions **using**. La différence entre les deux méthodes est que le compilateur de ligne de commande a besoin de l'emplacement du fichier d'assembly. La référence Visual Studio s'occupe de cela pour vous en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="7ce64-p103">The most common way to add a reference is to use Visual Studio. We know that some developers out there like to use other editors, so we are including instructions for using the command-line compiler as well as instructions for using Visual Studio. You might notice that the code examples that follow have the same **using** statements. The difference between the two methods is that the command-line compiler needs the location of the assembly file. The Visual Studio reference handles this for you behind the scenes.</span></span> 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a><span data-ttu-id="7ce64-119">Pour ajouter une référence à l'aide de Visual Studio</span><span class="sxs-lookup"><span data-stu-id="7ce64-119">To add a reference by using Visual Studio</span></span>

1. <span data-ttu-id="7ce64-p104">Placez le fichier Microsoft.Exchange.WebServices.dll et le fichier Microsoft.Exchange.WebServices.xml dans un dossier de votre choix. Par défaut, les fichiers sont installés dans  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, mais vous pouvez les stocker où vous voulez sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="7ce64-p104">Put the Microsoft.Exchange.WebServices.dll file and the Microsoft.Exchange.WebServices.xml file into a folder of your choice. By default, the files are installed in  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, but you can store the files anywhere on your computer.</span></span>
    
2. <span data-ttu-id="7ce64-p105">Dans le volet Explorateur de solutions dans Visual Studio, sélectionnez **Références**, puis choisissez **Ajouter une référence**. La fenêtre Ajouter une référence s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="7ce64-p105">In the Solution Explorer pane in Visual Studio, select **References**, and then choose **Add Reference**. This opens the Add Reference window.</span></span>
    
3. <span data-ttu-id="7ce64-124">Dans la fenêtre Ajouter une référence, accédez à l'onglet **Parcourir**, puis à l'emplacement du fichier Microsoft.Exchange.WebServices.dll, sélectionnez ce fichier, puis sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="7ce64-124">In the Add Reference window, navigate to the **Browse** tab, browse to the location of the Microsoft.Exchange.WebServices.dll file, select that file, and then select **OK**.</span></span> 
    
4. <span data-ttu-id="7ce64-125">Pour utiliser l'API managée EWS dans votre application, ajoutez une instruction **using** pour l'espace de noms **Microsoft.Exchange.WebServices.Data**.</span><span class="sxs-lookup"><span data-stu-id="7ce64-125">To use the EWS Managed API in your application, add a **using** statement for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a><span data-ttu-id="7ce64-126">Pour ajouter une référence et créer votre application avec le compilateur de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="7ce64-126">To add a reference and build your application with the command-line compiler</span></span>

1. <span data-ttu-id="7ce64-p106">Placez le fichier Microsoft.Exchange.WebServices.dll dans un dossier de votre choix. Ce dossier sera le dossier de sortie pour le compilateur.</span><span class="sxs-lookup"><span data-stu-id="7ce64-p106">Put the Microsoft.Exchange.WebServices.dll file into a folder of your choice. This folder will be the output folder for the compiler.</span></span>
    
2. <span data-ttu-id="7ce64-129">Dans votre éditeur de code source, ajoutez une instruction **using** au code source pour l'espace de noms **Microsoft.Exchange.WebServices.Data**.</span><span class="sxs-lookup"><span data-stu-id="7ce64-129">In your source code editor, add a **using** statement to the source code for the **Microsoft.Exchange.WebServices.Data** namespace.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. <span data-ttu-id="7ce64-p107">Exécutez le compilateur de ligne de commande pour créer l'application. La commande suivante utilise le compilateur C# .NET Framework pour créer l'application Windows définie dans le fichier de code source « program.cs ». Il suppose que le compilateur se trouve dans le répertoire d'installation par défaut et que le fichier Microsoft.Exchange.WebServices.dll est dans un sous-répertoire du répertoire en cours appelé « build ».</span><span class="sxs-lookup"><span data-stu-id="7ce64-p107">Run the command-line compiler to build the application. The following command uses the .NET Framework C# compiler to build the Windows application defined in the source code file "program.cs". It assumes that the compiler is located in the default installation directory and that the Microsoft.Exchange.WebServices.dll file is in a subdirectory of the current directory named "build".</span></span>
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a><span data-ttu-id="7ce64-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ce64-133">See also</span></span>

- [<span data-ttu-id="7ce64-134">Prise en main des applications clientes d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7ce64-134">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)    
- [<span data-ttu-id="7ce64-135">La configuration de votre environnement de développement d'applications Exchange</span><span class="sxs-lookup"><span data-stu-id="7ce64-135">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="7ce64-136">Communiquer avec EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7ce64-136">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

